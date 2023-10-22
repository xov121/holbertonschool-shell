```
0-current_working_directory
Prints the absolute path name of the current working directory.
pwd

1-listit
Displays the content list of the current directory.
ls

2-bring_me_home
Changes the working directory to the user's home directory.
cd ~

3-listfiles
Displays the current directory contents in a long format.
ls -l

4-listmorefiles
Displays current directory contents, including hidden files, in a long format.
ls -la

5-listfilesdigitonly
Displays current directory contents in a long format with user and group IDs displayed numerically. Also includes hidden files.
ls -lna

6-firstdirectory
Creates a directory named my_first_directory in the /tmp/ directory.
mkdir /tmp/my_first_directory

7-movethatfile
Moves the file betty from /tmp/ to /tmp/my_first_directory.
mv /tmp/betty /tmp/my_first_directory

8-firstdelete
Deletes the file betty that is located in /tmp/my_first_directory.
rm /tmp/my_first_directory/betty

9-firstdirdeletion
Deletes the directory my_first_directory that is in the /tmp directory.
rmdir /tmp/my_first_directory

10-back
Changes the working directory to the previous one.
cd -

11-lists
Lists all files in the current directory, the parent of the working directory, and the /boot directory in long format.
ls -la . .. /boot

12-file_type
Prints the type of the file named iamafile located in the /tmp directory.
file /tmp/iamafile

13-symbolic_link
Creates a symbolic link to /bin/ls, named __ls__ in the current working directory.
ln -s /bin/ls __ls__

14-copy_html
Copies all the HTML files from the current working directory to the parent directory. Only copies files that are newer or don't exist in the parent directory.
cp *.html ../

15-lets_move
Moves all files beginning with an uppercase letter to the directory /tmp/u.
mv [A-Z]* /tmp/u

16-clean_emacs
Deletes all files in the current working directory that end with the character ~.
rm *~

17-tree
Creates the directories welcome/, welcome/to/ and welcome/to/school in the current directory using only two spaces (and lines).
mkdir -p welcome/to/school
```
