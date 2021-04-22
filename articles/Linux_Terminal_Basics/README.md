# Linux Terminal Basics
## Here we will learn basics Linux terminal commands (using [Ubuntu](http://ubuntu.com))

___
# ls

Syntax:
`ls dir`

(Listing `dir`)

Example:

`ls /home`:

`user1 user2`


___

# cd

Syntax:
`cd dir`

(moving)

Example:

`user@device:~$ cd Desktop`

`user@device~/Desktop$ _`

___

# mkdir

Syntax:
`mkdir dir`

(Makes empty `dir` in selected directory)

Example:

`$ mkdir dir22`

`$ ls`

*`any_dir dir22`*

___

# rmdir

Syntax:
`rmdir dir`

(Removes *empty* `dir`)

Example:

`$ mkdir dir22`

`$ ls`

`any_dir dir22`

`$ ls dir22`

[Nothing]

`$ rmdir dir22`

`$ ls`

`any_dir`

___

# How to remove not empty dir or file? `rm`

Syntax:
`rm anything`

(Removes `anything` - file)

### Removing not empty dir:

`$ rm -r dir`

(`-r` - recursive)


