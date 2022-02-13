# Linux termial commands

### 1. `pwd`
This commands prints the absolute path to the current working directory and it's full form is print working directory.

### 2. `ls`
This command list the contents the content of the present working directory. It has many flags that you can find in help by providing<br> `ls --help`

### 3. `alias`
This command let you define aliases for the current session. The sytax is <br>
```
Syntax: alias name="value"
Example: alias ls="list-contents"

```
To see all the aliases type 'alias'

### 4. `unalias`
It is the opposite of the above command and removes the alias created.<br>
```
The below command with remove the alias created above
unalias ls
```

### 5. `cd`
It's full form is `change directory` and as names says it is used for changing the directory or the folder in very common terms trhough terminal.

```
1. To go into next directory use it like this `cd nameOfFolder`
Example: cd photos

2. To go into previous directory
cd .. 
and 
cd ../..  #to go two folders back and so on

3. By typing just `cd` it will take us to home folder

```

### 6 `cp`
This command is use to copy file and folders. To use it just type the soruce file/ foler and then destination file/folder

```
cp source-file.txt destination-file.txt
```
To copy directories use the (-r) recursive flag
```
cp -r source-folder/ destination-folder/
```
### 7 `rm`
This command is use to remove the files and the folders. It is a bit difficult to recover the files/folder deleted in this way.

```
rm file-to-remove.txt
```
To remove directories use the (-r) recursive flag
```
rm -r folder-to-remove/
```
### 8 `mv`
This command is use to move file/directories or rename it.

1. To rename the file
```
mv old-file.txt renamed-file.txt
```
2. To move the file
```
mv file.txt directory-name
```
3. To move all the file maching some pattern. Below example will move all the file with extension .js to javascript-files.
```
mv *.js /javascript-files 
```
4. You can move multiple file simultaneously.
```
mv first-file.txt second-file.txt /directory
```

### 9 `touch`
This command create the new empty file in the current directory.

```
touch newfile.txt
```
> Note: To create mutiple files at same time give names after one space.

### 10 `cat`

Concatenate(cat) command is used for various purpose like creating a file with content in it, viewing the contents, concatenation of content, coping the contents.

1. Create a file.
```
cat > file-name
```
3. Read the contents of file.
```
cat file-name
```
3. Copy the contents of file.
```
cat file-whose-content-is-to-be-copied > destination-file-name
```
4. Append the contens of one file to another
```
cat `fileName-whose-content-is-to-be-appended` >> `fileName-in-which-it-is-to-be-appended`
```

### 11. `mkdir`
This command is use to create the directory.

```
mkdir diretory-name
```
To create directory inside already existing directory give the (-p) parent tag.
```
mkdir -p parentDirectory/childDirectory
```

### 12 `man`
This commands shows the manual page for any command in linux even for itself.

```
man ls
```
For itself even
```
man man
```

### 13 `chmod` 
This command lets us change the permission or mode of the file.<br>
Three basic permissions are:
1. Read (r)
2. Write (w)
3. Execute (x)
To make the file executable type the below command
```
chmod +x file-name

```

### 14 `exit`
This is the very simple command as the name suggest by this command we can end the shell session and will automatically close the terminal.
```
exit
```
