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

    pwd   -  print current working directory path
    mkdir -  create directory
    rmdir -  remove/delete directory
    touch -  create a file
    rm    -  remove/delete file
    mv    -  rename file from one to another
    ls -a -  list hidden files
    cp    -  copy file/directory from one directory to another
    chmod -  modify permissions
    man   -  manual for any command
    grep  -  search inside files
    cat   -  print contents of whole file
    echo  -  repeat/print whatever comes after the command


---

### Q2.  List Files in Unix   

What do the following commands do:  

    ls    - list all files in the given directory
    ls -a - list all files including hidden files  
    ls -l - long format listing
    ls -lh - long format and human readable listing  
    ls -lah - long format, human readable listing of all files (including those hidden)
    ls -t  - list newest files first (timestamp based)
    ls -Glp - display colored long format listing, show directories with / in front of name


---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

    ls -lhaFg - display in long form, human readable, all files including hidden, flag file names, with color coded display

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

    xargs reads data from stdin and executes the command (given to it as an argument) one or more times based on the input read. Blanks and spaces are treated as delimiters, blank lines are ignored.
    Example: xargs can be used with find and grep. In this case, we find all text files, and filter out those which contain the word 'metis' in them.
    
    find -name '*.txt' | xargs grep 'metis'
