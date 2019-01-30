# Introduction to the Bash Command line

## Introduction
## Navigating through your file system

```
pwd #find out what directory you are in
ls #to get a listing of the files in your current location
man -ls #understand the flags, windows users use help
ls *.txt #search files matching a specific pattern
cd #explore the change directory command
```

**Test your understanding**

from the current location, navigate to the root location for linux users or desktop folder for windows users. list the files using the following arguments:
- use a long listing format
- sort by file size, largest first

*hint: use the man -ls to get the list of allowed arguments*


## Interacting with Files

##### Reading files

```
mkdir IntroShell-Text #create a new directory to engage with text files
cd IntroShell-Tex #or simply cd.. or cd IntroS with then hit tab to auto-complete
wget http://www.gutenberg.org/files/2600/2600-0.txt 
ls -lh #to check if the file is available
cat pg2600-0.txt #read the file within the command line environment
head pg2600-0.txt #read the head of the file
tail pg2600-0.txt #read the tail of the file
mv pg2600-0.txt mytext.txt #rename the file
```

##### Editing files


## Perform basic data manipulation tasks such as combining and copying files

##### Moving files


##### Coping files


##### Deleting files




