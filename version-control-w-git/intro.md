
##### What is Version control

a **system** that records changes to a file or a set of files over time so you can recall specific versions later. 

a version control system(VCS) allows you to:
- revert selected files back to a previous state
- revert an entire project back to a previous state
- compare changes over time
- see who last modified something that might be causing a problem
- who introduced an issue and when
- if you lose files, you can easily recover
- get all the above for very little overhead
- highly useful if you are into software development(source code), or simply if you work with files(spreadsheets, word docs, photoshop images etc)


##### types of version control systems

1. People's choice of version-control

Copy files into other directories (perhaps a time-stamped directory, if they're clever)

*   simple
*   incredibly error prone(accidently over-write/delete files etc)
*   difficult to keep a track of what changes were done
*   high overhead(a mess with many files)

2. Local VCS

has a simple database of patch sets(that is, the differences between files) in a special format on disk; it can then re-create what any file looked like at any point in time by adding up all the patches. 

![](images/localVCS.png)

```
sudo apt-get install rcs #install RCS
mkdir RCS #make a directory into which we can save the logs
ln -s ./RCS RCS #This links your working directory to the RCS repository
touch helloworld.sh #create a file that you want to maintain version control
vim #edit the file and save the file
ci helloworld.sh #When done editing the file, check-in (commit) your changes - It creates and/or writes to a file named helloworld.sh,v 
ls -sl | grep hello* #The grep command is used to search text
more helloworld.sh,v #to see what RCS has done to the file you checked-in
co -l helloworld.sh #latest version of the file "helloworld.sh " will be placed in your current working directory and "locked" from use by other programmers
co -u helloworld.sh #Check-out for reading not updating and locking
co -r1.2 helloworld.sh #To check-out a particular (previous) version
rcsdiff helloworld.sh #This will compare the version of the file in your working directory with that of the original you checked-out
rlog -b helloworld.sh #To view file info
```




2. Centralized VCS

- In RCS, the client needed to always checkout files with a lock if you want to make changes to them.

- RCS is working completely locally. Thus if you want to work on the same files with a team these files must be located on some shared disk or on some common server. 


![](images/centralizedVCS.png)

a singer server that contains all the versioned files and a number of clients that checkout files from the central place concurrently. 





3. Distributed VCS



*references*

1. Revision Control System(RCS)-http://jodypaul.com/SWE/RCSTutorial/RCSTutorial.html

2. Getting started about version control-https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control