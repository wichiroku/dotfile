[[color codes cmd.png]]

```
==================== 1. NAVIGATION ====================

dir                         Lists files and folders
cd folder                   Enters the specified folder
cd ..                       Goes to the parent folder
cd \                        Goes to the root of the current drive
cd /d D:\Projects           Switches to D: drive and enters Projects
D:                          Switches to the D: drive
cls                         Clears the CMD screen
tree                        Displays folders in a tree structure
```

```
==================== 2. CREATE FILES AND FOLDERS ====================

mkdir Projects              Creates a folder named Projects
echo Hello                  Prints Hello in CMD
echo Hello > file.txt       Creates file.txt containing Hello; overwrites if it exists
echo World >> file.txt      Appends World to file.txt
type file.txt               Displays the contents of file.txt

type nul > file.txt         Creates an empty text file
copy nul file.txt           Creates an empty file
notepad file.txt            Opens Notepad; prompts to create the file if needed
```


```
==================== 3. COPY, MOVE AND RENAME ====================

copy a.txt b.txt            Copies a.txt into a new file named b.txt
move a.txt Projects         Moves a.txt into the Projects folder
ren old.txt new.txt         Renames old.txt to new.txt
```

```
==================== 4. DELETE FILES AND FOLDERS ====================

del file.txt                Deletes file.txt
rmdir Projects              Deletes Projects if the folder is empty
rmdir /s Projects           Deletes Projects and all its contents; asks for confirmation
rmdir /s /q Projects        Deletes Projects and all its contents without confirmation
```


```
==================== 5. SYSTEM INFORMATION ====================

whoami                      Displays your Windows username
hostname                    Displays your computer's name
ipconfig                    Displays network configuration
ver                         Displays Windows version information
help                        Lists available CMD commands
mkdir /?                    Displays help for the mkdir command
exit                        Closes CMD
```


```
==================== 6. OPEN FILES AND APPLICATIONS ====================

start .                     Opens the current folder in File Explorer
explorer .                  Opens the current folder in File Explorer
start notepad file.txt      Opens file.txt in Notepad
code .                      Opens the current folder in VS Code, if configured
```


```
==================== 7. CHANGE CMD COLORS ====================

color XY                    Changes background (X) and text (Y) colors
```