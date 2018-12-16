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

> > pwd - print working directory
ls - list with options and location
cd - change directory
file - to check file type
man - to look up command info
mkdir - make directory
rmdir - remove directory
touch - create a file
mv - move a file
cat - view a file
chmod - modify permissions 

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

> > the backtick can save the output of a command to a variable
ls  lists the items in the current directory
ls -a  lists the contents of a directory including hidden files
ls -l   List in long format the total sum for all the file sizes is output before
ls -lh   When used with the -l option, use unit suffixes: Byte, Kilobyte,
             Megabyte, Gigabyte, Terabyte and Petabyte in order to reduce the
             number of digits to three or less using base 2 for sizes.
ls -lah  long list including those that begin with dot and the unit suffixes
ls -t   sorts by the time modified
ls -Glp   enables colorized output and a slash after each file name

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > -r  displays in reverse order
-1  displays each entry on one line
-F Flags filenames
-R displays subdirectories as well
-m displays as comma sep list

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > xargs can run a particular command for every item in a list. 
can make directories or files out a string of data
echo 'one two three' | xargs mkdir
ls
one two three

or remove them 'one two three' | xargs rmdir
with one line swift and easy

 

