---
id: yec6m8mw1va3gubn8vy63d8
title: Bash and Terminal
desc: ""
updated: 1703685098350
created: 1703536700694
---

Bash is a command line interpreter language that lets us interact with our operating system.

- These commands work in `wsl`: Windows Subsystem for Linux
- Can be installed by running: `wsl --install` in admin cmd.

1. **pwd** : print working directory
2. **cd** : change directory, `cd ..` to get one folder before
3. **ls** : list directory
   - `-l` with `ls` to get details about the contents
   - `-R` (recursively) gives details of all the sub directories as well
   - `-t` orders as per last modified.
   - These commands can be combined too, like `-lt` gives details of files in the order of last modified with timestamp of modification.
   - `-la` to view hidden files, their names are preceded by `.`.
   - `-r` gives files in reverse order of last modified.
   - `-s` size based listing
   - `grep file_type` / `*.file_type`: wildcard, to get files of a certain file type
   - wildcard can also be used as regex to get certain files
4. **mdkir** : make directory/folder
   - `&&` operator can be used to perform another operation with `mkdir`.
5. **touch** : create a file
6. **cat** : prints contents of a file
   - can also be used to change/concatenate data to an existing file, like `cat > file_name.txt`. `>>` to append at the end of the file.
7. **vi** : to edit directly in terminal(Not recommended)
   - To save & exit this, `Esc`-> `:wq` -> `:wq!`
8. **mv** : move files -> `mv move_folder/file destination_folder`
   - Used to rename too: `mv inital_name new_name`
9. **cp** : copy files (like mv)
   - to copy folder add `-r` flag between command and file
10. **rm** : remove
11. **nvm** : Node Version Manager
12. **npm** : Node Package Manager ( Downloads external dependencies)
13. **node** : Gives a playground to run nodejs directly in terminal
    - `node file_name`: runs a JS File
14. **chmod** : change file permissions
    - `chomd ugo+rwx`
    - u: user | g: group | o: others
    - permissions- r: read | w: write | x: execute
    - add `-R` for folders
    - Ex: `chmod g+wx file.sh`: means write & execute permissions are given to group for file.sh
    - `chmod u-x file2.txt` means user got his execute permissions revoked for file2.txt
    - A numeric method of permission change through chmod is also there.
15. **echo** : cmd's print statement
    - to view current path : `echo $PATH`
16. **head & tail** : to view the respective positions of a file
    - add `-20` to view only
      the command's repsective content
17. `|` : pipe character, whtever result is produced by the command before it flows through the command written after it
18. **wc** : to get word/line/char count - we can get occurenece of something with `grep` and then gwt the number of occureneces by combining `wc` with pipe operator.
    `-r` for every 'not recommended' option.

19. **grep** : searches for the pattern specified by the Pattern parameter and writes each matching line to standard output. [More info](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

20. **history** : gives history of the all the commands run

21. **bash script** : we can make scripts using bash

    - For that first line of the script should specify: `#!/bin/bash`.
    - Then we can run it by : `bash file_name.sh`

22. **sed** : Stream Editor. Sed helps in operations like selecting the text, substituting text, modifying an original file, adding lines to text, or deleting lines from the text.

    - Syntax: `sed OPTIONS [SCRIPT] [INPUTFILENAME]`
    - _Options_ control the output of the Linux command
    - _Script_ contains a list of Linux commands to run
    - _File name (with extension)_ represents the file on which you’re using the sed command.
    - [More info](https://www.geeksforgeeks.org/sed-command-in-linux-unix-with-examples/)

23. **awk**: Awk is a utility that enables a programmer to write tiny but effective programs in the form of statements that define text patterns that are to be searched for in each line of a document and the action that is to be taken when a match is found within a line. Awk is mostly used for pattern scanning and processing.
    - Syntax: `awk options 'selection _criteria {action }' input-file > output-file`
    - Can also help in cherrypicking columnar data like csv files with some particular conditonal statements
    - [More Info](https://www.geeksforgeeks.org/awk-command-unixlinux-examples/)
