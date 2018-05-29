# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar: 
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > 
Action | Command
----------------|----------------
show current working directory path | pwd
creating a directory | mkdir <dirname>
deleting a directory | rmdir <dirname /s
creating a file using `touch` command | touch <filename>
deleting a file | rm <filename>
renaming a file | mv <oldname> <newname>
listing hidden files | ls -ld .?\* 
copying a file from one directory to another | cp <filename> <dirname>
modify file permissions | chmod <755,+x,+r,+w>
view file contents | cat <filename>


---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

> > `ls` lists the files in a directory (not hidden files)**
`ls -a`  lists all files in a directory, including hidden files**
`ls -l`  lists files in long format (permissions, etc are shown)**
`ls -lh` lists files in long format with a readable file size**
`ls -lah` lists all files in long format with a readable file size, including hidden files**
`ls -t`   lists files sorted by time and date**
`ls -Glp` lists files in long format, ommitting group designations (owner names), and appending a slash '/' to directories
---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > 'ls -R' lists subdirectories as well**
'ls -u' sorts files by access time**
'ls -t' sorts files by newest (based on timestamp)**
'ls -x' displays files as rows across the screen**
'ls -d' displays only directories**


---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > 'xargs' is a command that takes in Standard Input (which results from another function) and executes a command using each element of the Standard Input. The following example shows how to find and delete all '.txt' extension files in the directory /foo:**
find ./foo -type f -name "\*.txt" | xargs rm

 

