```
0-hello_world
Prints "Hello, World" followed by a new line to the standard output.
printf 'Hello, World\n'

1-confused_smiley
Displays a confused smiley "(Ôo)'.
printf  "\"(Ôo)'\n"

2-hellofile
Displays the content of the /etc/passwd file.
cat /etc/passwd

3-twofiles
Displays the content of /etc/passwd and /etc/hosts.
cat /etc/passwd /etc/hosts

4-lastlines
Displays the last 10 lines of /etc/passwd.
tail -n 10 /etc/passwd

5-firstlines
Displays the first 10 lines of /etc/passwd.
head -n 10 /etc/passwd

6-third_line
Displays the third line of the file iacta.
head -3 iacta | tail -1

7-file
Creates a file named exactly *\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text "Best School" ending by a new line.
echo -e "Best School" > "\\*\\\\'\"Best School\"\\'\\\\*\$\\?\\*\\*\\*\\*\\*:)"

8-cwd_state
Writes the result of ls -la into the file ls_cwd_content.
ls -la > ls_cwd_content

9-duplicate_last_line
Duplicates the last line of the file iacta.
tail -n 1 iacta >> iacta

10-no_more_js
Deletes all .js files in the current directory and its subfolders.
find . -name "*.js" -type f -delete

11-directories
Counts the number of directories and sub-directories in the current directory.
find . -type d ! -name '.' -print |wc -l

12-newest_files
Displays the 10 newest files in the current directory.
ls -t | head -n 10

13-unique
Prints only words that appear exactly once from a list of words.
sort | uniq -u

14-findthatword
Displays lines containing the pattern "root" from /etc/passwd.
cat /etc/passwd | grep root

15-countthatword
Displays the number of lines that contain the pattern "bin" in /etc/passwd.
cat /etc/passwd | grep bin | wc -l

16-whatsnext
Displays lines containing the pattern "root" and the three lines following them in /etc/passwd.
grep -A 3 root /etc/passwd

17-hidethisword
Displays lines in /etc/passwd that do not contain the pattern "bin".
grep -Av bin /etc/passwd

18-letteronly
Displays lines in /etc/ssh/sshd_config starting with a letter.
grep '^[A-Za-z]' /etc/ssh/sshd_config

19-AZ
Replaces all characters A and c from input to Z and e respectively.
tr 'A c' 'Z e'

20-hiago
Removes all letters c and C from input.
tr -d 'cC'

21-reverse
Reverses its input.
rev

22-users_and_homes
Displays all users and their home directories, sorted by users.
cut -d ':' -f '1,6' /etc/passwd | sort
```
