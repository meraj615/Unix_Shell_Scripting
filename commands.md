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
jithendra
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
/home/jithendra/projects
```

### `cd`
**Purpose:**
```
Moves to home directory
```

### `cd .`
**Purpose:**
```
Stay in the same directory (no change).
```

### `cd ..`
**Purpose:**
```
Move one level up
```

### `cd ~`
**Purpose:**
```
Go to home directory.
```

### `cd /home`
**Purpose:**
``` bash
Moves to the /home directory
```

### `cd -`
**Purpose:**
``` bash
Switches back to the previous working directory
```

#### Listing Files & Directories ######
### `ls`
**Purpose:** 

```bash
Lists files and directories in the current directory.
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
**Purpose:** 

```bash
Lists all files, including hidden files (files starting with .).
```

### `ls -lh`
**Purpose:** 

```bash
Lists files in long format with human-readable file sizes (KB, MB, GB).
```

### `ls -ltr`
**Purpose:** 

```bash
Lists files in long format, sorted by modification time (oldest first).
```

### `ls -ltrh`
**Purpose:** 

```bash
Lists files in long format, sorted by time, with human-readable sizes
```

### `ls -ltra`
**Purpose:** 

```bash
Lists all files (including hidden) in long format, sorted by time.
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

