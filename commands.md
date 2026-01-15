#### `Basic Commands For Linux/Commands for the Data Engineer` #########
#### `System Information Commands` ######

### `uname`
**Purpose:** Shows complete system information (kernel, OS, architecture).

```bash
uname -a
```

**Output:** 
```
  Linux server01 5.15.0-91-generic #101-Ubuntu SMP x86_64 GNU/Linux
```

### `whoami`
**Purpose:** Displays the current logged-in user.

```bash
whoami
```
**Output:**
```
meraj
```

### `hostname`
**Purpose:** Shows the system’s host name.

```bash
hostname
```
**Output:**
```
server01
```

### `date`

**Purpose:** Shows current system date and time.

```bash
date
```
**Output:*** 
```
Tue Jan 13 14:05:22 EST 2026
```

### `uptime`
**Purpose:** Shows how long the system has been running.

```bash
uptime
```
**Output:**
```
14:05:30 up 12 days, 4:32, 2 users, load average: 0.15, 0.10, 0.08
```


### File & Directory Management ###

### `pwd`
**Purpose:** Prints current working directory.

```bash
pwd
```
**Output:**
```
/home/meraj/projects
```

### `cd`
**Purpose:** Moves to home directory
```bash
cd
```


### `cd .`
**Purpose:** Stay in the same directory (no change).
```bash
cd .
```

### `cd ..`
**Purpose:**Move one level up
```
cd ..
```

### `cd ~`
**Purpose:** Go to home directory.
```
cd ~
```

### `cd /home`
**Purpose:** Moves to the /home directory
``` bash
cd /home
```

### `cd -`
**Purpose:** Switches back to the previous working directory
``` bash
cd -
```

#### Listing Files & Directories ######
### `ls`
**Purpose:** Lists files and directories in the current directory.

```bash
ls
```
### `ls -l`
**Purpose:** Lists files and directories in long format (permissions, owner, size, date).

```bash
ls -l
```
**Output:** 
```
  -rw-r--r-- 1 user user  4096 Jan 13  data.csv
  drwxr-xr-x 2 user user  4096 Jan 12  logs

```
### `ls -a`
**Purpose:** Lists all files, including hidden files (files starting with .).

```bash
ls -a
```

### `ls -lh`
**Purpose:** Lists files in long format with human-readable file sizes (KB, MB, GB).

```bash
ls -lh
```

### `ls -ltr`
**Purpose:** Lists files in long format, sorted by modification time (oldest first).

```bash
ls -ltr
```

### `ls -ltrh`
**Purpose:** Lists files in long format, sorted by time, with human-readable sizes 

```bash
ls -ltrh
```

### `ls -ltra`
**Purpose:** Lists all files (including hidden) in long format, sorted by time.

```bash
ls -ltra
```

### Directory Creation & Removal ###

### `mkdir`
**Purpose:** Creates a new directory.

```bash
mkdir dir_name
```

### `rmdir`
**Purpose:** Removes an empty directory.

```bash
rmdir dir_name
```

### File Creation & Copy Commands ###

### `touch`
**Purpose:** Creates an empty file or updates the timestamp of an existing file.

```bash
touch file_name
```

### `touch file1 file2`
**Purpose:** Creates multiple empty files at once.

```bash
touch file1 file2
```

### `cp`
**Purpose:** Copies a file to another file.

```bash
cp file1 file2
```

### `cp file1 dir1`
**Purpose:** Copies a file into a directory.

```bash
cp file1 dir1
```

### `cp file1 file2 file3 dir1`
**Purpose:** Copies multiple files into a directory.

```bash
cp file1 file2 file3 dir1
```

### `cp -r1`
**Purpose:** Copies a directory recursively.

```bash
cp -r dir1 dir2
```

### `cp -i`
**Purpose:** Prompts before overwriting an existing file.

```bash
cp -i file1 file2
```

### `cp -u`
**Purpose:** Copies only when the source file is newer than the destination.

```bash
cp -u file1 file2
```

### `cp -a`
**Purpose:** Copies directories while preserving permissions, ownership, and timestamps.

```bash
cp -a dir1 dir2
```

### `cp -rf`
**Purpose:** Forces recursive copy and overwrites existing files without prompt.

```bash
cp -rf dir1 dir2
```

### File Move & Rename Commands ###

### `mv`
**Purpose:** Moves or renames files and directories.

```bash
mv file1 file2
```

### `mv file1 /home/`
**Purpose:** Moves a file to another directory.

```bash
mv file1 /home/
```


### `mv /home/file1 /home/file2`
**Purpose:** Renames a file within the same directory.

```bash
mv /home/file1 /home/file2
```

### File & Directory Removal Commands ###


### `rm`
**Purpose:** Removes (deletes) a file.

```bash
rm file_name
```


### `rm -i`
**Purpose:** Prompts for confirmation before deleting a file.

```bash
rm -i file_name
```


### `rm -r`
**Purpose:** Removes a directory and its contents recursively.

```bash
rm -r dir_name
```


### `rm -f`
**Purpose:** Forces file deletion without confirmation.

```bash
rm -f file_name
```


### `rm -rf`
**Purpose:** Forces recursive deletion of directories and files without prompt.

```bash
rm -rf dir_name
```

### File & Directory Search Commands ###

### `find .`
**Purpose:** Lists all files and directories from the current directory.

```bash
find .
```
**Output:** 
```
 .
./file1
./dir1
./dir1/file2
```


### `find . -type f`
**Purpose:** Finds only files in the current directory and subdirectories.

```bash
find . -type f
```
**Output:** 
```
./file1
./dir1/file2
```

### `find . -type d`
**Purpose:** Finds only directories in the current directory and subdirectories.

```bash
find . -type d
```
**Output:** 
```
.
./dir1
```


### `cat`
**Purpose:** Displays the contents of a file.

```bash
cat file_name
```
**Output:** 
```
Hello World
Welcome to Linux
This is a sample file
```


### `cat file1 file2`
**Purpose:** Displays the contents of multiple files sequentially.

```bash
cat file1 file2
```
**Output:** 
```
Content of file1
Line 2 of file1
Content of file2
Line 2 of file2
```


### `cat -n`
**Purpose:** Displays file content with line numbers.

```bash
cat -n file_name
```
**Output:** 
```
     1  Hello World
     2  Welcome to Linux
     3  This is a sample file
```



### `head`
**Purpose:** Displays the first 10 lines of a file.

```bash
head file_name
```
**Output:** 
```
     Line 1
    Line 2
    Line 3
    ......
    Line 10
```



### `head -n`
**Purpose:** Displays the specified number of lines from the beginning of a file.

```bash
head -n 5file_name
```
**Output:** 
```
  Line 1
  line 2
  .....
  line 5
```


### `tail`
**Purpose:** Displays the last 10 lines of a file.
```bash
tail file_name
```
**Output:** 
```
  Line 91
  line 92
  .....
  line 100
```


### `tail -n`
**Purpose:** Displays the specified number of lines from the end of a file.

```bash
tail -n 5 file_name
```
**Output:** 
```
  Line 95
  line 96
  .....
  line 100
```

### `tail -f`
**Purpose:** Continuously displays new lines added to a file (useful for log monitoring).

```bash
tail -f file_name
```
**Output:** 
```
 [INFO] Application started
 [INFO] Processing request
 [INFO] Request completed
```


### VI Editor Commands ###

### `vi`
**Purpose:** Opens a file in the vi editor.
```bash
vi file_name
```

### `vi`
**Purpose:** Opens a file in the vi editor.
```bash
vi file_name
```

### `vi +10`
**Purpose:** Opens the file and places the cursor on line 10.
```bash
vi +10 file_name
```


### `vi +/pattern`
**Purpose:** Opens the file and jumps to the first occurrence of a pattern.
```bash
vi +/pattern file_name
```

### `vi -R`
**Purpose:** Opens the file in read-only mode.
```bash
vi -R file_name
```


### Save & Exit Commands within vi editor ###
### `:w `
**Purpose:** Saves the current file.
```bash
:w
```

### `:q`
**Purpose:** Quits vi (only if no changes were made).
```bash
:q
```


### `:q!`
**Purpose:** Quits vi without saving changes.
```bash
:q!
```

### `:wq`
**Purpose:** Saves the file and exits vi.
```bash
:wq
```


### `:x`
**Purpose:** Saves the file (only if modified) and exits.
```bash
:x
```


### `ZZ`
**Purpose:** Saves the file and exits vi (shortcut).
```bash
ZZ
```

### Insert Mode Commands within Vi editor ###

### `i`
**Purpose:** Inserts text before the cursor.
```bash
i
```

### `I`
**Purpose:** Inserts text at the beginning of the line.
```bash
I
```


### `a`
**Purpose:** Appends text after the cursor.
```bash
a
```


### `A`
**Purpose:** Appends text at the end of the line.
```bash
A
```

### `o`
**Purpose:** Opens a new line below the current line.
```bash
o
```

### `O`
**Purpose:** Opens a new line above the current line.
```bash
O
```


### `Esc`
**Purpose:** Exits insert mode and returns to command mode.
```bash
Esc
```


### Cursor Movement Commands within vi editors###
### `h`
**Purpose:** Moves cursor left.
```bash
h
```

### `j`
**Purpose:** Moves cursor down.
```bash
j
```

### `k`
**Purpose:** Moves cursor up.
```bash
k
```


### `l`
**Purpose:** Moves cursor right.
```bash
l
```


### `w`
**Purpose:** Moves to the beginning of the next word.
```bash
w
```


### `b`
**Purpose:** Moves to the beginning of the previous word.
```bash
b
```

### `e`
**Purpose:** Moves to the end of the current word.
```bash
e
```


### `0`
**Purpose:** Moves to the beginning of the line.
```bash
0
```


### `^`
**Purpose:** Moves to the first non-blank character of the line.
```bash
^
```


### `$`
**Purpose:** Moves to the end of the line.
```bash
$
```


### `gg`
**Purpose:** Moves to the first line of the file.
```bash
gg
```

### `G`
**Purpose:** Moves to the last line of the file.
```bash
G
```


### `:n`
**Purpose:** Moves to line number n.
```bash
:n
```


### Delete Commands within Vi editor ###
### `x`
**Purpose:** Deletes the character under the cursor.
```bash
x
```

### `dw`
**Purpose:** Deletes a word from the cursor position.
```bash
dw
```

### `dd`
**Purpose:** Deletes the entire current line.
```bash
dd
```


### `d$`
**Purpose:** Deletes from cursor to end of the line.
```bash
d$
```


### `dG`
**Purpose:** Deletes from cursor to end of the file.
```bash
dG
```

### Copy (Yank) & Paste Commands within vi editor ###
### `yy`
**Purpose:** Copies the current line.
```bash
yy
```


### `yw`
**Purpose:** Copies a word.
```bash
yw
```

### `y$`
**Purpose:** Copies from cursor to end of the line.
```bash
y$
```


### `p`
**Purpose:** Pastes copied text after the cursor.
```bash
p
```


### `P`
**Purpose:** Pastes copied text before the cursor.
```bash
P
```

### Undo & Redo within Vi Editor ###

### `u`
**Purpose:** Undoes the last change.
```bash
u
```

### `Ctrl + r`
**Purpose:** Redoes the undone change.
```bash
Ctrl + r
```

### Search Commands within Vi Editor ###
### `/pattern`
**Purpose:** Searches forward for a pattern.
```bash
/pattern
```


### `?pattern`
**Purpose:** Searches backward for a pattern.
```bash
?pattern
```

### `n`
**Purpose:** Moves to the next search result.
```bash
n
```


### `N`
**Purpose:** Moves to the previous search result.
```bash
N
```

### Replace Commands within Vi Editor ###
### `:s/old/new/`
**Purpose:** Replaces first occurrence of text in the current line.
```bash
:s/old/new/
```


### `:s/old/new/g`
**Purpose:** Replaces all occurrences in the current line
```bash
:s/old/new/g
```

### `:%s/old/new/g`
**Purpose:** Replaces all occurrences in the entire file.
```bash
:%s/old/new/g
```


### `:%s/old/new/gc`
**Purpose:** Replaces with confirmation for each match.
```bash
:%s/old/new/gc
```

### Line Number Settings within Vi Editor ###

### `:set number`
**Purpose:** Displays line numbers.
```bash
:set number
```


### `:set nonumber`
**Purpose:** Hides line numbers.
```bash
:set nonumber
```

### Visual Modes in Vi Editor ###

### `v`
**Purpose:** Starts character-wise visual mode.
```bash
v
```


### `V`
**Purpose:** Starts line-wise visual mode.
```bash
V
```

### `Ctrl + v`
**Purpose:** Starts block-wise visual mode.
```bash
Ctrl + v
```

### Indentation within Vi Editor ###

### `>>`
**Purpose:** Indents the current line to the right.
```bash
>>
```

### `<<`
**Purpose:** Indents the current line to the left.
```bash
<<
```


### File & Buffer Commands within Vi Editor ###

### `:e`
**Purpose:** Opens another file in the same editor.
```bash
:e filename
```

### `:bn`
**Purpose:** Switches to the next buffer.
```bash
:bn
```

### `:bp`
**Purpose:** Switches to the previous buffer.
```bash
:bp
```

### Execute Shell Commands from vi ###

### `:!ls`
**Purpose:** Runs the ls command from vi.
```bash
:!ls
```

### `:!pwd`
**Purpose:** Runs the pwd command from vi.
```bash
:!pwd
```


### grep – Search Text in Files ###

### `grep`
**Purpose:** Searches for a pattern in a file and displays matching lines.

```bash
grep pattern file_name
```
**Output:** 
```
This line contains pattern
```

### `grep -i`
**Purpose:** Performs a case-insensitive search.

```bash
grep -i pattern file_name
```
**Output:** 
```
Pattern found in this line
```


### `grep -r`
**Purpose:** Searches recursively in all files under the current directory.

```bash
grep -r pattern .
```
**Output:** 
```
./file1:pattern found here
./dir1/file2:another pattern
```


### `grep -n`
**Purpose:** Displays matching lines with line numbers.

```bash
grep -n pattern file_name
```
**Output:** 
```
12:This line contains pattern
```

### `grep -v`
**Purpose:** Displays lines that do NOT contain the pattern.
```bash
grep -v pattern file_name
```
**Output:** 
```
This line does not match
Another unrelated line
```


### `grep -w`
**Purpose:** Matches the exact word only.

```bash
grep -w pattern file_name
```
**Output:** 
```
pattern
```

### `grep -c`
**Purpose:** Counts the number of matching lines.

```bash
grep -c pattern file_name
```
**Output:** 
```
3
```


### `grep -l`
**Purpose:** Displays file names that contain the pattern.

```bash
grep -l pattern *
```
**Output:** 
```
file1
file3
```


### `grep -H`
**Purpose:** Displays the file name with matching lines.

```bash
grep -H pattern file_name
```
**Output:** 
```
file_name:This line contains pattern
```

### `grep -o`
**Purpose:** Displays only the matched part of the line.
```bash
grep -o pattern file_name
```
**Output:** 
```
pattern
```


### `grep -E`
**Purpose:** Searches using extended regular expressions.

```bash
grep -E "pat1|pat2" file_name
```
**Output:** 
```
This line has pat1
This line has pat2
```

### `grep -F`
**Purpose:** Searches for a fixed string (no regex interpretation).

```bash
grep -F "fixed_string" file_name
```
**Output:** 
```
fixed_string found here
```


### `grep -A`
**Purpose:** Displays matching lines and 3 lines after the match.

```bash
grep -A 3 pattern file_name
```
**Output:** 
```
This line contains pattern
Next line
Next line
Next line
```

### `grep -B`
**Purpose:** Displays matching lines and 3 lines before the match.
```bash
grep -B 3 pattern file_name
```
**Output:** 
```
Previous line
Previous line
Previous line
This line contains pattern
```


### `grep -C`
**Purpose:** Displays matching lines with 3 lines before and after.

```bash
grep -C 3 pattern file_name
```
**Output:** 
```
Previous line
Previous line
Previous line
This line contains pattern
Next line
Next line
Next line
```


### sed – Stream Editor ###

### `sed 's/old/new/'`
**Purpose:** Replaces the first occurrence of old with new in each line.

```bash
sed 's/old/new/' file_name
```
**Output:** 
```
This is new text
old value remains here
```

### `sed 's/old/new/g'`
**Purpose:** Replaces all occurrences of old with new in each line

```bash
sed 's/old/new/g' file_name
```
**Output:** 
```
new value new value
```


### `sed 's/old/new/2'`
**Purpose:** Replaces only the second occurrence of old in each line.
```bash
sed 's/old/new/2' file_name
```
**Output:** 
```
old new old
```


### `sed 's/old/new/gI'`
**Purpose:** Replaces all occurrences case-insensitively.

```bash
sed 's/old/new/gI' file_name
```
**Output:** 
```
new NEW new
```

### `sed -i 's/old/new/g'`
**Purpose:** Replaces text in the file itself (in-place edit).
```bash
sed -i 's/old/new/g' file_name
```
**Output:** 
```
No output File modified directly
```


### `sed -n '5p'`
**Purpose:** Prints only line 5 of the file.

```bash
sed -n '5p' file_name
```
**Output:** 
```
This is line 5
```

### `sed -n '1,10p'`
**Purpose:** Prints lines 1 through 10.

```bash
sed -n '1,10p' file_name
```
**Output:** 
```
Line 1
Line 2
...
Line 10
```


### `sed '5d'`
**Purpose:** Deletes line 5 from the output.

```bash
sed '5d' file_name
```
**Output:** 
```
Line 1
Line 2
Line 3
Line 4
Line 6
```


### `sed '1,10d'`
**Purpose:** Deletes lines 1 through 10.

```bash
sed '1,10d' file_name
```
**Output:** 
```
Line 11
Line 12
```

### `sed '/pattern/d'`
**Purpose:** Deletes lines that match a pattern.
```bash
sed '/pattern/d' file_name
```
**Output:** 
```
Lines without pattern
```


### `sed '/pattern/p'`
**Purpose:** Prints lines matching the pattern along with all lines.

```bash
sed '/pattern/p' file_name
```
**Output:** 
```
Normal line
pattern line
pattern line
```

### `sed -n '/pattern/p'`
**Purpose:** Prints only lines that match the pattern.
```bash
sed -n '/pattern/p' file_name
```
**Output:** 
```
pattern found here
```


### `sed 's/^/START-/'`
**Purpose:** Adds text at the beginning of each line.
```bash
sed 's/^/START-/' file_name
```
**Output:** 
```
START-Line one
START-Line two
```

### `sed 's/$/-END/'`
**Purpose:** Adds text at the end of each line.
```bash
sed 's/$/-END/' file_name
```
**Output:** 
```
Line one-END
Line two-END
```


### `sed 's/[0-9]//g'`
**Purpose:** Removes all digits from the file output.

```bash
sed 's/[0-9]//g' file_name
```
**Output:** 
```
Order number 
```

### `sed 's/^[[:space:]]*//'`
**Purpose:** Removes leading spaces from each line.
```bash
sed 's/^[[:space:]]*//' file_name
```
**Output:** 
```
Text without leading spaces
```


### `sed 's/[[:space:]]*$//'`
**Purpose:** Removes trailing spaces from each line.

```bash
sed 's/[[:space:]]*$//' file_name
```
**Output:** 
```
Text without trailing spaces
```


### awk – Pattern Scanning & Processing Language ###

### `awk '{print}'`
**Purpose:** Prints every line of the file.
```bash
sed 's/old/new/' file_name
```
**Output:** 
```
John 25 USA
Alice 30 UK
```

### `awk '{print $1}'`
**Purpose:** Prints the first column of each line

```bash
awk '{print $1}' file_name
```
**Output:** 
```
John
Alice
```


### `awk '{print $1,$2}'`
**Purpose:** Prints the first and second columns.
```bash
awk '{print $1,$2}' file_name
```
**Output:** 
```
John 25
Alice 30
```


### `awk '{print NR,$0}'`
**Purpose:** Prints line numbers along with each line.

```bash
awk '{print NR,$0}' file_name
```
**Output:** 
```
1 John 25 USA
2 Alice 30 UK
```

### `awk -F',' '{print $1}'`
**Purpose:** Uses comma as the field separator and prints the first field.
```bash
awk -F',' '{print $1}' file_name
```
**Output:** 
```
John
Alice
```


### `awk '/pattern/ {print}'`
**Purpose:** Prints lines that match a specific pattern.

```bash
awk '/pattern/ {print}' file_name
```
**Output:** 
```
This line contains pattern
```

### `awk '{sum+=$1} END {print sum}'`
**Purpose:** Calculates and prints the sum of values in the first column.

```bash
awk '{sum+=$1} END {print sum}' file_name
```
**Output:** 
```
150
```

### cut – Extract Sections from Each Line ###

### `cut -d',' -f1`
**Purpose:** Extracts the first field using comma as the delimiter.

```bash
cut -d',' -f1 file_name
```
**Output:** 
```
John
Alice
Mark
```

### `cut -c1-5`
**Purpose:** Extracts characters from position 1 to 5.

```bash
cut -c1-5 file_name
```
**Output:** 
```
Hello
World
```

### sort – Sort Lines of Text ###

### `sort`
**Purpose:** Sorts file content in ascending (alphabetical) order.

```bash
sort file_name
```
**Output:** 
```
Alice
John
Mark
```

### `sort -r`
**Purpose:** Sorts file content in reverse order.

```bash
sort -r file_name
```
**Output:** 
```
Mark
John
Alice
```

### `sort -n`
**Purpose:** Sorts numbers in numeric order.

```bash
sort -n file_name
```
**Output:** 
```
10
25
100
```


### uniq – Filter Adjacent Duplicate Lines ###
### uniq works correctly only on sorted files ###

### `uniq`
**Purpose:** Removes adjacent duplicate lines.

```bash
uniq file_name
```
**Output:** 
```
Apple
Banana
Orange
```

### `uniq -c`
**Purpose:** Counts occurrences of each line.

```bash
uniq -c file_name
```
**Output:** 
```
2 Apple
1 Banana
3 Orange
```

### `uniq -d`
**Purpose:** Displays only duplicate lines.

```bash
uniq -d file_name
```
**Output:** 
```
Apple
Orange
```

### wc – Word, Line, and Character Count ###

### `wc`
**Purpose:** Displays line, word, and byte counts.
```bash
wc file_name
```
**Output:** 
```
 10  50  300 file_name
```

### `wc -l`
**Purpose:** Displays number of lines.

```bash
wc -l file_name
```
**Output:** 
```
10
```

### `wc -w`
**Purpose:** Displays number of words.
```bash
wc -w file_name
```
**Output:** 
```
 50
```

### `wc -c`
**Purpose:** Displays number of bytes (characters).

```bash
wc -c file_name
```
**Output:** 
```
300
```

### chmod – Change File Permissions ###

### `chmod 755`

**Purpose:** Sets permissions to rwxr-xr-x
Owner: read, write, execute
Group: read, execute
Others: read, execute

```bash
chmod 755 file_name
```


### `chmod u+x`
**Purpose:** Adds execute permission to the file owner.

```bash
chmod u+x file_name
```

### chown – Change File Ownership ###

### `chown user:group`
**Purpose:** Changes both owner and group of a file.
```bash
chown user:group file_name
```

### chgrp – Change Group Ownership ###

### `chgrp group`
**Purpose:** Changes the group ownership of a file.

```bash
chgrp group file_name
```


