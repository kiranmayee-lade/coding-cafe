Question 1 
What did --global mean here? What would happen if you left it out? Guess, then check with man git-config or ask.

Answer: -—global saves the variable information in a global scope. If —global was left out, it would not be accessible throughout the scope of the program. 

Verifying with man git-config:
--global
           For writing options: write to global ~/.gitconfig file rather than the repository .git/config, write to $XDG_CONFIG_HOME/git/config file if this file exists and the ~/.gitconfig file doesn’t.

           For reading options: read only from global ~/.gitconfig and from $XDG_CONFIG_HOME/git/config rather than from all available files.

           See also the section called “FILES”.

In Git, the --global flag means that the configuration option you are setting will apply to all Git repositories for your user account on your computer.


Question 2 
What appeared in ls -a but not in ls? What is inside it?

Answer: Ls -a included .venv and .git along with the files and directories that were previously worked on(README.md week01 and week02)

Question 3 
Roughly how many files and folders is Git offering to track? Does anything in that list look like something you did not write?

Answer: Git is offering to track 2 files


Question 4 Compare this git status with the one from Question 3. What disappeared?

Answer: My files under venv were not visible in the previous 'git status' as well. 

Question 5
.gitignore itself shows up as untracked. Should it be committed, or ignored too? Why?

.gitignore is currently ignored as its contents are not tracked by Git. .gitignore should be committed because Git needs to track the file to ensure that everyone working on the repository uses the same rules for which files Git should ignore. 

Question 6
README.md moved from one heading to another in the git status output. Which two? In the three-places model from the session, what just happened to it?

Answer: README.md moved from untracked files to Changes to be committed. In the three-places model, it was first tracked by git, and then 'committed' to allow a snapshot of README.md to be added to the timeline.

Question 7
What did Git print after the commit? How many files did it say changed?

 3 files were changed, 74 insertions(+)

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
This represents a commit hash, they are used for uniquely identifying an individual commit within one specific project. 

Question 9
You now have two commits. Without looking it up: what are the four steps of the loop you just did twice?

Step 1 add the filename to the tracked files list
Step 2 commit the filename and use -m to add a comment
Step 3 check git status
Step 4 check git log --oneline

After looking up the loop, the correct order is to start with a git status.

Question 10
Why does this file get a special name and a special place, rather than being called notes.md like everything else?

README.md is in the root directory and it gets a special identifier and place because GitHub automatically recognizes it as the main introduction for a project (collaborators can immediately see information about the project)


Question 11
What did gh auth login do that means you will not be asked for a password when you push?
It performed Authentication of Git with my GitHub account and stored the authentication credentials. 

Question 12
Refresh the repository page on GitHub. What is showing on the front page, and why that file?

Answer: The list of committed files is visible and the complete content of README.md is displayed. README.md is displayed on the front page as GitHub recognizes the file name as the main documentation for a project and it is used to present the primary information about the repository to the collaborators and users.  

Question 13
Run git log --oneline again. Did pushing change your local history in any way?

Answer: Performing a push did not change the local history

Question 14
Your repository is private but your TAs can now read it. In your own words, what is the difference between a repository being private and a repository not existing on GitHub at all?

Answer: A private repository is accessible only to the owner and the collaborators that are invited. It is available for edits and viewing on the GitHub platform. 

A repository that does not exist on GitHub is local to the owner's device and has not yet been connected and pushed to the user's GitHub account. 