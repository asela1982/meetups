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
code pg2600-0.txt #open the file using the program Visual Studio Code
cat pg2600-0.txt #read the file within the command line environment
head pg2600-0.txt #read the head of the file
tail pg2600-0.txt #read the tail of the file
mv pg2600-0.txt mytext.txt #rename the file
```

##### Editing files


## Perform basic data manipulation tasks such as combining and copying files

##### Combining files

```
cp pg2600-0.txt tolstoy.txt #duplicate a file
cp tolstoy.txt tolstoy2.txt #to combine
cat tolstoy.txt tolstoy2.txt #to combine two or more files but prints the output within the shell
cat tolstoy.txt tolstoy2.txt > tolstoy-twice.txt #send the output to a newfile
cat *.txt > everything-together.txt #combining more than two files
```

##### Coping and Moving files

basic format of the copy command: cp [source] [destination]
if you dont want to leave a copy behind, replace cp with mv

```
cp tolstoy.txt tolstoy-backup.txt #create a backup
cp /home/asela/Documents/tolstoy.txt /home/asela/Downloads/ #move a file
cp /home/asela/Documements/*.txt /home/asela/Downloads/
#move several files at once
cp /home/asela/Downloads/tolstoy.txt ./
# ./ command refers to the current directory you are in
```


##### Deleting files




