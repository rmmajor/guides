# Terminal commands

---
## BASICS

    path which starts with '/' is absolute, if not, it is relative
    '/' is a root dir (root of a filesystem tree)
    
    1 tab helps enter the comand or finish path, 2 tabs shows the options to end comand/path
    
    .. - the dir above (parent dir)
    . - the current dir

---
## COMMANDS FOR FILESYSTEM

### cd - Change Directory
    cd somefolder/some_sub_folder/ # Change Directory 
    cd .. # go 1 dir up
    cd # moves to home dir
    cd ~ # also moves to home dir

### ls - lists all files in the dir
    ls [dir name] # lists the content of that dir without entering it
    ls ~ # lists contents of your home dir, no matter where you are
    ls -R # lists all files within children dirs recursively

### pwd - print working directory
 (shows absolute path to current dir)

### cp - copy
WARNING: If there already was a file called duplicate.txt, it is overwritten

    cp original.txt duplicate.txt 
    cp dir1/file1.csv dir1/file2.csv dir2 # would copy both files and file2 into dir2
    
### mv - move 
WARNING: mv will overwrite existing files (can by useful but also dangerous)

    mv dir1/file1.csv dir1/file2.csv dir2 # would move both files and file2 into dir2
    mv name1.txt name2.txt # renames a file

### rm - remove, delete
    rm file.txt # deletes a file
    rm file1.txt file2.txt # deletes a banch of files

### _mkdir_ and _rmdir_
    mkdir dir_name # makes new empty dir
    rmdir # deletes an empty(!) dir

### cat - shows a content of a file in terminal (no editing)

    cat file.txt
    cat -n file.txt # cat with lines counted

### less - allows you to read and scrole files in terminal 
    less file1.txt file2.txt # shows files in tabs 
	:n - to next file
	:q - to quit

### head and tail 

    head file.txt # shows 10 first lines of a file 
    head -n file.txt # shows n first lines of a file 
    tail file.txt # does the same but from the end

### cut displays files by their columns (kind of vertical head)
    
    cut -f1 -d; filename.scv # selects first col with ; as a separator

### grep - search in files by keyphrases

    grep "key phrase" file.txt # shows all the rows that contain the key phrase
    grep -c "key phrase" file.txt # shows count of rows that contain the key phrase
    grep -v "key phrase" file.txt # shows all the rows that DONT contain the key phrase

## OTHER USEFUL COMMANDS 

### man
    man [command_name] # displays a manual for the command

### instaling packages in ubuntu
    sudo apt install [package_name] # installs a package from a repository apt

### history 
    history # shows all indexed comands you`ve entered
    ![n] # reruns n-th comand from history list
