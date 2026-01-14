#### Basic Commands For Linux/Commands for the Data Engineer #########
#### System Information Commands ######

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
**Sample Output:*** 
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
