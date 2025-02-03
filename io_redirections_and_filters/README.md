# I/O Redirections and Filters

This directory contains a collection of Bash scripts that demonstrate various techniques for input/output redirections and text filtering.

## Scripts

### 0-hello_world
**Task:** Prints "Hello, World" followed by a new line to the standard output.
**Example:** `echo "Hello, World"`

### 1-confused_smiley
**Task:** Displays a confused smiley: "(Ôo)'".
**Example:** `echo "(Ôo)'"`

### 2-hellofile
**Task:** Displays the content of `/etc/passwd`.
**Example:** `cat /etc/passwd`

### 3-twofiles
**Task:** Displays the content of `/etc/passwd` and `/etc/hosts`.
**Example:** `cat /etc/passwd /etc/hosts`

### 4-lastlines
**Task:** Displays the last 10 lines of `/etc/passwd`.
**Example:** `tail -n 10 /etc/passwd`

### 5-firstlines
**Task:** Displays the first 10 lines of `/etc/passwd`.
**Example:** `head -n 10 /etc/passwd`

### 6-third_line
**Task:** Displays the third line of the file `iacta`.
**Example:** `head -n 3 iacta | tail -n 1`

### 7-file
**Task:** Creates a file named exactly `*\'"Best School"\'\*0******:)` containing "Best School" followed by a new line.
**Example:** `echo "Best School" > "*\'\"Best School\"\'\*0******:)"`

### 8-cwd_state
**Task:** Writes the output of `ls -la` into the file `ls_cwd_content`, overwriting it if it exists.
**Example:** `ls -la > ls_cwd_content`

### 9-duplicate_last_line
**Task:** Duplicates (appends) the last line of the file `iacta` to the end of the file.
**Example:** `tail -n 1 iacta >> iacta`

### 10-no_more_js
**Task:** Deletes all regular files with a `.js` extension in the current directory and its subfolders.
**Example:** `find . -type f -name "*.js" -delete`

### 11-directories
**Task:** Counts the number of directories (and subdirectories) in the current directory (excluding . and .., including hidden directories).
**Example:** `find . -mindepth 1 -type d | wc -l`

### 12-newest_files
**Task:** Displays the 10 newest files in the current directory, one per line, sorted from newest to oldest.
**Example:** `ls -t1 | head -n 10`

### 13-unique
**Task:** From a list of words given via standard input (one per line), prints only those words that appear exactly once, sorted alphabetically.
**Example:** `sort | uniq -u`

### 14-findthatword
**Task:** Displays lines containing the pattern "root" from `/etc/passwd`.
**Example:** `grep "root" /etc/passwd`

### 15-countthatword
**Task:** Counts the number of lines in `/etc/passwd` that contain the pattern "bin".
**Example:** `grep "bin" /etc/passwd | wc -l`

### 16-whatsnext
**Task:** Displays lines containing "root" and the 3 lines following each match from `/etc/passwd`.
**Example:** `grep -A 3 "root" /etc/passwd`

### 17-hidethisword
**Task:** Displays all lines in `/etc/passwd` that do not contain the pattern "bin".
**Example:** `grep -v "bin" /etc/passwd`

### 18-letteronly
**Task:** Displays all lines in `/etc/ssh/sshd_config` that start with a letter (A–Z or a–z).
**Example:** `grep "^[A-Za-z]" /etc/ssh/sshd_config`

### 19-AZ
**Task:** Replaces all occurrences of the character **A** with **Z** and **c** with **e** in the input.
**Example:** `tr 'Ac' 'Ze'`

### 20-hiago
**Task:** Removes all occurrences of the letters **c** and **C** from the input.
**Example:** `tr -d 'cC'`

### 21-reverse
**Task:** Reverses the input text.
**Example:** `rev`

### 22-users_and_homes
**Task:** Displays all users and their home directories from `/etc/passwd`, sorted by username.
**Example:** `cut -d ':' -f1,6 /etc/passwd | sort -t ':' -k1,1`

### 23-empty_casks
**Task:** Lists the names (without paths) of all empty files and directories in the current directory tree.
**Example:** `find . -empty | rev | cut -d'/' -f1 | rev`

### 24-gifs
**Task:** Lists all `.gif` files (from the current directory and subdirectories) without their extension, sorted case-insensitively.
**Example:** `find . -type f -iname "*.gif" | sed 's/\.[gG][iI][fF]$//' | sort -f`

### 25-acrostic
**Task:** Decodes an acrostic by printing the first letter of each input line.
**Example:** `awk '{printf "%s", substr($0,1,1)} END {print ""}'`

### 26-the_biggest_fan
**Task:** Parses TSV log input and displays the 11 hosts or IP addresses that made the most requests.
**Example:** `tail -n +2 | cut -f1 | sort | uniq -c | sort -k1,1nr | head -n 11 | awk '{print $2}'`
