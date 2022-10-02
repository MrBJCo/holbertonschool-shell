# Shell, permissions
## My name is Betty 
### (0-iam_betty) Create a script that switches the current user to the user betty.
#### #!/bin/bash
su betty
## Who am I 
### (1-who_am_i) Write a script that prints the effective username of the current user.
#### #!/bin/bash
whoami
## Groups 
### (2-groups) Write a script that prints all the groups the current user is part of.
#### #!/bin/bash
groups
## New owner
### (3-new_owner) Write a script that changes the owner of the file hello to the user betty.
#### #!/bin/bash
sudo chown betty hello
## Empty! 
### (4-empty) Write a script that creates an empty file called hello.
#### #!/bin/bash
touch hello
## Execute 
### (5-execute) Write a script that adds execute permission to the owner of the file hello
#### #!/bin/bash
chmod u+x hello
## Multiple permissions 
### (6-multiple_permissions) Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.
#### #!/bin/bash
chmod 754 hello
## Everybody! 
### (7-everybody) Write a script that adds execution permission to the owner, the group owner and the other users, to the file hello
#### #!/bin/bash
chmod ugo+x hello
## James Bond
### (8-James_Bond) Write a script that sets the permission to the file hello as follows: the owner and group (no permisions), Others users (have permision)
#### #!/bin/bash
chmod 007 hello
## John Doe 
### (9-John_Doe) Write a script that sets the mode of the file hello to this: the file hello will be in the working directory, You are not allowed to use commas for this sript
#### #!/bin/bash
chmod 753 hello
## Look in the mirror 
### (10-mirror_permissions) Write a script that sets the mode of the file hello the same as olleh’s mode.
#### #!/bin/bash
chmod --reference=olleh hello
## Directories 
### (11-directories_permissions) Create a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.
#### #!/bin/bash
chmod a+x */
## More directories
### (12-directory_permissions) Create a script that creates a directory called my_dir with permissions 751 in the working directory.
#### #!/bin/bash
mkdir -m 751 my_dir
## Change group 
### (13-change_group) Write a script that changes the group owner to school for the file hello
#### #!/bin/bash
chgrp school hello
## Owner and group 
### (14-change_owner_and_group) Write a script that changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.
#### #!/bin/bash
chown vincent:staff *
## Symbolic links
### (15-symbolic_link_permissions) Write a script that changes the owner and the group owner of _hello to vincent and staff respectively.
#### #!/bin/bash
chown -h vincent:staff _hello
## If only 
### (16-if_only) Write a script that changes the owner of the file hello to vincent only if it is owned by the user guillaume.
#### #!/bin/bash
chown --from=guillaume vincent hello
