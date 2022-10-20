# Homework 2: Unix shell

This homework will assess your ability to run commands in the shell and make a simple script.

Replace the lines specified in _italics_ with your answers and save as a text file.


## Problem 0

**60 points**

Complete the interactive tutorial.

_Did you hit any points of frustration, and if so, how could we improve the material to avoid that frustration?_  

Yes, I encountered many points of frustration.  I have zero coding/computer language experience, so the learning curve for me is quite steep and simple things take me hours to try and figure out.  Also, I continually received errors and commands not found during the tutorial.  I routinely had to google the error, and try to troubleshoot by installing different commands by running many different scripts, most of which did not work.  A classmate suggested I open a new terminal outside of vscode to view some of the commands (like man man), and then it worked.  But that seems to slightly defeat the purpose to have resources be differentially available depending on whether you are in vscode or not?  I think another frustration is that I never know if what I am doing is correct or successful.  OVerall I enjoy learnig all the new things, I just have no idea what I'm doing, ha   


## Problem 1

**20 points**

**Write a script that outputs some user and location data and moves that output to a newly created directory**

Make a single script that prints out a file called question01.txt. 

This file should contain the following text:

  My name is (your username, but the script needs to work for anyone, not just you)

  My home directory is (your home directory, but the script needs to work for anyone, not just you)

  The contents of the tfcb_2022/lectures/lecture04/ directory are

  (prints the contents of that directory)

This script should also create a directory called homework02, and move question01.txt into the homework02 directory.

Example:
My name is melody
My home directory is /Users/melody
The contents of the tfcb_2022/lectures/lecture04/ directory are
01-first-steps.md
02-directories
03-redirection
04-vim
05-history
06-scripting
07-more-interactive-shell
README.md
quickref.md
sequence.gb
slides
vader.txt

#!/bin/bash
FILENAME=${question01}
echo my name is $user
mkdirmy name is and my home directory is The contents of the tfcb_2022/lectures/lecture04/ directory are README.md homeworks lectures reference.md software tfcb-homework02
echo my name is $user and my home directory is $home The contents of the tfcb_2022/lectures/lecture04/ directory are $(ls) > question01.txt
mkdir homework02
mv question01.txt homework02


## Problem 2

**20 points**

**Write a script that uses a loop to output files with specific names**


Make a single script that does the following:

Makes a new directory in homework02 called question02

In that directory, your script should make 25 new files called
file###.txt

the ### should be the numbers from a list you can find here:

tfcb_2022/homeworks/homework02/list.txt

You can make the contents of those files whatever you want (hint: slide 10... what was the contents of the fake "jpg" file?)


