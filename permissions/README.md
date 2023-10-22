```
0-iam_betty
Switches the current user to the user betty. Assumes that user betty exists.
su betty

1-who_am_i
Prints the effective username of the current user.
whoami

2-groups
Prints all the groups the current user is a part of.
groups

3-new_owner
Changes the owner of the file hello to the user betty.
chown betty hello

4-empty
Creates an empty file named hello.
touch hello

5-execute
Adds execute permission to the owner of the file hello.
chmod u+x hello

6-multiple_permissions
Adds execute permission to the owner and the group owner, and read permission to other users, for the file hello.
chmod ug+x,o+r hello

7-everybody
Adds execution permission to the owner, the group owner, and other users for the file hello.
chmod ugo+x hello

8-James_Bond
Sets the permission for the file hello as follows: Owner and Group have no permission, Other users have all permissions.
chmod 007 hello

9-John_Doe
Sets the mode of the file hello to -rwxr-x-wx.
chmod 753 hello

10-mirror_permissions
Sets the mode of the file hello the same as the file olleh.
chmod --reference=olleh hello

11-directories_permissions
Adds execute permission to all subdirectories of the current directory for the owner, the group owner, and all other users. Regular files are not changed.
find . -type d -exec chmod a+x {} +

12-directory_permissions
Creates a directory called my_dir with permissions 751.
mkdir -m 751 my_dir

13-change_group
Changes the group owner to school for the file hello.
chgrp school hello

14-change_owner_and_group
Changes the owner to vincent and the group owner to staff for all files and directories in the working directory.
chown vincent:staff *

15-symbolic_link_permissions
Changes the owner and the group owner of the symbolic link _hello to vincent and staff respectively.
chown -h vincent:staff _hello

16-if_only
Changes the owner of the file hello to vincent only if it is owned by the user guillaume.
chown --from=guillaume vincent hello
```
