# Shell, permissions
## My name is Betty 
### (0-iam_betty) Create a script that switches the current user to the user betty.
#### #!/bin/bash
echo -e "Hello, World"
## Who am I 
### (1-who_am_i) Write a script that prints the effective username of the current user.
#### #!/bin/bash
echo "\"(Ôo)'"
## Groups 
### (2-groups) Write a script that prints all the groups the current user is part of. 
#### #!/bin/bash
cat /etc/passwd
## New owner 
### (3-new_owner) Write a script that changes the owner of the file hello to the user betty.
#### #!/bin/bash
cat /etc/passwd /etc/hosts
## Empty! 
### (4-empty) Write a script that creates an empty file called hello.
#### #!/bin/bash
tail -n 10 /etc/passwd
## Execute 
### (5-execute) Write a script that adds execute permission to the owner of the file hello.
#### #!/bin/bash
head -n 10 /etc/passwd
## Multiple permissions 
### (6-multiple_permissions) Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.
#### #!/bin/bash
head -n 3 iacta | tail -n 1
## Everybody! 
### (7-everybody) Write a script that adds execution permission to the owner, the group owner and the other users, to the file hello
#### #!/bin/bash
echo "Best School" > "\*\\\'\"Best School\"\'\\\*$\?\*\*\*\*\*:)"
## James Bond 
### (8-James_Bond) Write a script that sets the permission to the file hello as follows: Owner and Group no permission at all, Other users: all the permissions
#### #!/bin/bash
ls -la > ls_cwd_content
## John Doe
### (9-John_Doe) Write a script that sets the mode of the file hello
#### #!/bin/bash
tail -n 1 iacta >> iacta
## Look in the mirror 
### (10-mirror_permissions) Write a script that sets the mode of the file hello the same as olleh’s mode
#### #!/bin/bash
find -type f -name "*.js" -delete
## Directories
### (11-directories_permissions) Create a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.
#### #!/bin/bash
find . -mindepth 1 -type d | wc -l
## More directories
### (12-directory_permissions) Create a script that creates a directory called my_dir with permissions 751 in the working directory.
#### #!/bin/bash
ls -t1 |head -n 10
## Change group 
### (13-change_group) Write a script that changes the group owner to school for the file hello
#### #!/bin/bash
sort | uniq -u
## Owner and group 
### (14-change_owner_and_group) Write a script that changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.
#### #!/bin/bash
grep 'root' /etc/passwd
## Symbolic links 
### (15-symbolic_link_permissions) Write a script that changes the owner and the group owner of _hello to vincent and staff respectively
#### rep -c -i "bin" -A 3 /etc/passwd  
## If only 
### (16-if_only) Write a script that changes the owner of the file hello to vincent only if it is owned by the user guillaume.
#### #!/bin/bash
grep -i "root" -A 3 /etc/passwd
