Question 1
pwd is the present working directory. Using this command displays the folder that the user is currently working in. 

Question 2
ls -a revealed files that were hidden in plain ls, such as files starting with a period .

Question 3
-rw-r--r--@   1 kiranmayeelade  staff     326 12 Aug 23:11 lecture1.c

Question 4
I was in the home folder (cd ~) and it works because the week02 folder is a part of the home directory. coding-cafe/week02 is a relative path. 


Question 5
The command mv moved README-backup.md from the coding-cafe directory into the week01 directory. 
The command mv then renamed README-backup.md to the file name old-readme.md


Question 6
There are 10 folders

Question 7
/Library/Frameworks/Python.framework/Versions/3.13/bin/python3

Question 8 
/usr/bin/python3
The PATH is different. My friend's is the Python installed/provided inside their Linux environment, whereas mine is through Python 3.13 installation.

Question 9 
zsh: command not found: pyton3
PATH is a special list of folders on the computer. The PATH included Python3, and the system looks for that exact name in each directory. pyton3 does not exist in the PATH  so the shell reports that the command cannot be found. 

Question 10
ls does not display files starting with a period such as .venv

Question 11
The shell adds the name of the box (.venv) or environment to the start of the terminal prompt.

Question 12
/Users/kiranmayeelade/coding-cafe/.venv/bin/python3
This path is different from the one displayed in Step 7. A different location (environment) of python3 is started to be used

Question 13
5 different packages were added, including 'requests' and 'charset-normalizer'

Question 14
/Library/Frameworks/Python.framework/Versions/3.13/bin/python3
It points back to the environment displayed in Step 7

Question 15
When used with the -l option, use unit suffixes: Byte, Kilobyte, Megabyte, Gigabyte, Terabyte and Petabyte in order to reduce the number of digits to four or fewer using base 2 for sizes.  This
             option is not defined in IEEE Std 1003.1-2008 (“POSIX.1”).

The -h command, used with -l, can display bytes into easily understandable units (suffixes) like Kilobytes (K), Megabytes (M), and Gigabytes (G) based on powers of 1024. In comparison to -l in Step 1, which displayed raw size of data, -h gives more shorthand, recognized notation of size. 

Question 16
Control+C showed a KeyboardInterrupt whereas Control+D returned to zsh

