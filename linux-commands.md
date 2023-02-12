# Linux Commands

## File / Directory Manipulation

### cat

- displays file contents

### cd

- Change current directory to home directory or specified directory
- `cd ../` go to previous directory
- `cd ../../` go to directory two levels up
- `cd -` go to previous working directory

### cp

- Copy files and directories
- By default, if the destination file exists, it will be overwritten
- `cp sourceFileName destFileName` copy file
- `cp -r sourceFileName destFileName` copy a directory, including all its files and subdirectories

### ls

#### `ls`

- shows only the names of the files and directories
- doesn’t list the hidden files by default

#### `ls -l`

- print files in a long listing format

#### `ls -a`

- display all files, including the hidden files

### mv

- Rename and move any files and directories from one location to another
- `mv fileName /newDirectory`   move a file to new directory
- `mv fileName newFileName`     rename file
- `mv fileName1 fileName2 /newDirectory` move multiple files to new directory

### mkdir

- `mkdir directory_name`    Create new directory
- `mkdir -p dir1/dir2/dir3` Create nested directories

### pwd 

- present working directory (pwd)
- find out the `current directory` you are working in

### rm

- `rm <<fileName>>`             Remove empty file
- `rm -d <<directoryName>>`     Remove empty directory
- `rm -rf <<directoryName>>`    Remove non-empty directory with files recursively

### sudo

- Elevate privilleges
- Run programs as another user, by default the root user

## touch

- `touch <<filename>>` creates file

## vim

### Editing Commands

- `vim <<filename>>` - Opens file in readonly mode. Create new if not exist.
- `i`   - Insert at cursor (goes into insert mode)
- `a`   - Write after cursor (goes into insert mode)
- `A`   - Write at the end of line (goes into insert mode)
- `Esc` - Terminate insert mode
- `u`   - Undo last change
- `U`   - Undo all changes to the entire line
- `o`   - Open a new line (goes into insert mode)
- `dd`  - Delete line
- `3dd` - Delete 3 lines.
- `D`   - Delete contents of line after the cursor
- `C`   - Delete contents of a line after the cursor and insert new text. 
- `dw`  - Delete word
- `4dw` - Delete 4 words
- `cw`  - Change word
- `x`   - Delete character at the cursor
- `r`   - Replace character
- `R`   - Overwrite characters from cursor onward
- `s`   - Substitute one character under cursor continue to insert
- `S`   - Substitute entire line and begin to insert at the beginning of the line
- `~`   - Change case of individual character

### Moving within a file

- `k` – Move cursor up
- `j` – Move cursor down
- `h` – Move cursor left
- `l` – Move cursor right


### Saving and Closing the file

- `Shift+zz`    – Save the file and quit
- `:w`          – Save the file but keep it open
- `:q!`         – Quit vi and do not save changes
- `:wq`         – Quit vi and save change before closing

## Networking

## ssh

### Connecting to EC2 Instance

```
Syntax:     ssh -i file.pem username@ip-address
Example:    ssh - pubkey.pem adarsh@10.20.43.56
```

- **ssh**: Command to use SSH protocol
- **i**: Flag that specifies an alternate identification file to use for public key authentication.
- **username**: Username that uses your instance
- **ip-address**: IP address given to your instance

### Other ssh Commands

#### ssh-keygen

- Creates a key pair for public key authentication

#### ssh-copy-id

- configures a public key as authorized on a server

#### ssh-agent

— agent to hold private key for single sign-on

#### ssh-add

— tool to add a key to the agent

#### scp

— file transfer client with RCP-like command interface

#### sftp

— file transfer client with FTP-like command interface

#### sshd

— OpenSSH server






