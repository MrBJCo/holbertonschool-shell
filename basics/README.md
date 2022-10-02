## Where am I?...
### (0-current_working_directory) Write a script that prints the absolute path name of the current working directory
####  #!/bin/bash
pwd
## What’s in there?
### (1-listit) Display the contents list of your current directory.
####  #!/bin/bash
ls
## There is no place like home 
### (2-bring_me_home) Write a script that changes the working directory to the user’s home directory
####  #!/bin/bash
cd
## The long format 
### (3-listfiles) Display current directory contents in a long format
#### #!/bin/bash
ls -l
## Hidden files 
### (4-listmorefiles) Display current directory contents, including hidden files (starting with .). Use the long format.
#### #!/bin/bash
ls -la
## I love numbers
### (5-listfilesdigitonly) Display current directory contents - (Long format, with user and group IDs displayed numerically and hidden files [starting with (.)])
#### #!/bin/bash
ls -na
## Welcome
### (6-firstdirectory) Create a script that creates a directory named my_first_directory in the /tmp/ directory.
#### #!/bin/bash
mkdir /tmp/my_first_directory
## Betty in my first directory
### (7-movethatfile) Move the file betty from /tmp/ to /tmp/my_first_directory.
#### #!/bin/bash
mv /tmp/betty /tmp/my_first_directory
## Bye bye Betty 
### (8-firstdelete) Delete the file betty - The file betty is in /tmp/my_first_directory
#### #!/bin/bash
rm /tmp/my_first_directory/betty 
## Bye bye My first directory 
### (9-firstdirdeletion) Delete the directory my_first_directory that is in the /tmp directory.
#### #!/bin/bash
rmdir /tmp/my_first_directory
## 10-back
### (10-back) Write a script that changes the working directory to the previous one.
#### #!/bin/bash
cd -
## Lists 
### (11-lists) Write a script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format.
#### #!/bin/bash
ls -la . .. /boot
## File type
### (12-file_type) Write a script that prints the type of the file named iamafile. The file iamafile will be in the /tmp directory when we will run your script.
#### #!/bin/bash
file /tmp/iamafile
## We are symbols, and inhabit symbols
### (13-symbolic_link) Create a symbolic link to /bin/ls, named __ls__. The symbolic link should be created in the current working directory.
#### #!/bin/bash
ln -s /bin/ls __ls__
## Copy HTML files 
### (14-copy_html) Create a script that copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory.
#### #!/bin/bash
cp -u *.html ..
## Let’s move
### (15-lets_move) Create a script that moves all files beginning with an uppercase letter to the directory /tmp/u. - You can assume that the directory /tmp/u will exist when we will run your script.
#### #!/bin/bash
mv [[:upper:]]* /tmp/u
## Clean Emacs 
### (16-clean_emacs) Create a script that deletes all files in the current working directory that end with the character (~).
#### #!/bin/bash
rm *~
## Tree
### (17-tree) Create a script that creates the directories welcome/, welcome/to/ and welcome/to/school in the current directory. - You are only allowed to use two spaces (and lines) in your script, not more.
#### #!/bin/bash
mkdir -p welcome/to/school
