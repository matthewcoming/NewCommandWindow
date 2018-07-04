# New Command Window

This is an extremely simple bash script that allows you to execute a command and all of it's arguments in a new terminal FROM the terminal.

## setup
1. Download ncw.sh from this repo, or copy the raw file into a text editor and save it.

2. Change the files permissions (I promise the file isn't `sudo rm -rf /`) using the command 
```Bash
$ chmod 755 ncw.sh
```
3. Move the file to any path stored in `$PATH`. The paths are seperated by colons.
```Bash
$ echo $PATH
/home/matt/bin:/home/matt/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/
$ mv ./ncw.sh /usr/local/bin/ncw
```
By moving the file to `/usr/local/bin` without the `.sh` filetype, we can call `ncw` like any other command.


## How to use it

If you wanted to edit a document called `myDocument.md` with vim in a new terminal, simple preface `vi myDocument.md` with the `ncw` command

```Bash
$ ncw vi myDocument.md
```

