# Linux Terminal Basics
## Here we will learn basics Linux terminal commands (using [Ubuntu](http://ubuntu.com))
___
`ls dir` - listing `dir`

`ls` - listing selected (*this*) dir


# Files

`cd dir` - selects `dir`

`cd` - selects `/home`

`cd /` - selects "root"/main dir

`cd ../` - selects parent dir

`pwd` - shows current dir

`mkdir dir` - making **empty** `dir` *here*

`rmdir dir` - removing only **empty** `dir`'s, else: error

`rm -r dir` - removing `dir` recursive (with files, too)

`touch file` - making or updating **empty** `file`

`rm file` - removing `file`

`cat file` - shows `file`

`less file` - shows `file` (full window)

`nano file` - opening `file` in NANO editor

\*nano: `Ctrl+O` - save, nano:`Ctrl+X` - close

`vi file` - opening `file` in VIM editor

\*After opening `vi`, press \[I] (**I**nsert) to edit file. Press \[esc] than type ":wq" to save and exit (`:q` - **Q**uit, `:w` - **W**rite)

`mv file1 file2` - extracts `file1` to `/` as `file2` (Renames file)

`mv file1 dir/` - extracts `file1` to `dir`

`cp file1 file2` - copies `file1` as `file2` to *here*

`cp file1 dir/` - copies `file1` to `dir`

# Users

`sudo adduser username` - adds user. It'll ask new password etc...

`sudo useradd username` - same as `adduser`, but doesnt asks password etc...

`sudo deluser username` - deletes user.

`sudo userdel username` - same as `deluser`.

`sudo passwd username` - change password for user.

\* If in `/home` is folder of deleted user: `cd /home` > `sudo rm -r userdir`

# Networking

`ping host` - ping `host`

`wget url` - downloads files from `url` *here*

`wget -r url` - downloads webpage from `url` recursively 

`curl url` - outputs webpage from `url`

`curl -o file.html url` - writes the page from `url` to `file.html`

# System info

`date` - shows date, time for *now*

`uptime` - shows uptime

`whoami` - who are you logged in as

`w` - shows, who's online


#### So. It's all basic commands for using Ubuntu PC without UI (in Terminal), thank you for attention.
