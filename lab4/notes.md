Question 1 What did --global mean here? What would happen if you left it out? Guess, then check with man git-config or ask.

Answer: -—global saves the variable information in a global scope. If —global was left out, it would not be accessible throughout. 

--global
           For writing options: write to global ~/.gitconfig file rather than the repository .git/config, write to $XDG_CONFIG_HOME/git/config file if this file exists and the ~/.gitconfig file doesn’t.

           For reading options: read only from global ~/.gitconfig and from $XDG_CONFIG_HOME/git/config rather than from all available files.

           See also the section called “FILES”.


Question 2 What appeared in ls -a but not in ls? What is inside it?
Ls -a included .venv and .git along with the files and directories that were previously worked on(README.md week01 and week02)

Question 3 Roughly how many files and folders is Git offering to track? Does anything in that list look like something you did not write?

Answer: Git is offering to track 2 files


Q4. Compare this git status with the one from Question 3. What disappeared?

Answer: My files under venv were previously not visible as well

Question 5: .gitignore itself shows up as untracked. Should it be committed, or ignored too? Why?

.gitignore should be ignored as the contents are not tracked. 

Question 6
README.md moved from one heading to another in the git status output. Which two? In the three-places model from the session, what just happened to it?

Answer: README.md moved from untracked files to Changes to be committed. In the three-places model, it was ‘committed’ and will be tracked by git, a snapshot of README.md is added to the timeline.

Question 7
What did Git print after the commit? How many files did it say changed?

 3 files changed, 74 insertions(+)

It printed
git commit -m "Lab work so far"
[main bd6edaf] Lab work so far
 3 files changed, 74 insertions(+)
 create mode 100644 README.md
 create mode 100644 week02/lab01-log.txt
 create mode 100644 week02/notes.md

Question 8
What are the first seven characters of your commit called, and what are they for?

Git log —oneline displays 
bd6edaf 
This represents a commit hash, they are used for uniquely identifying an individual commit within one specific project

Question 9

Step 1 add the filename to the tracked files list
Step 2 commit the filename and use -m to add a comment
Step 3 check git status
Step 4 check git log --oneline