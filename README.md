# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 

# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\MyLab
```
![8 o1](https://github.com/varshinidevaraju/Windows-basic-commands-batchscript/assets/144870750/719a4374-1c71-4a63-aef1-b1f4e4db2037)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![8 o2 1](https://github.com/varshinidevaraju/Windows-basic-commands-batchscript/assets/144870750/e715fee2-7c98-4120-8499-8f0c33195fa1)


![8 o 2 2](https://github.com/varshinidevaraju/Windows-basic-commands-batchscript/assets/144870750/1562ad8a-3374-4281-afdb-31d81a52f74d)




List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![8 os 3 1](https://github.com/varshinidevaraju/Windows-basic-commands-batchscript/assets/144870750/e74c2770-8e6e-40b6-9857-9143ebce6adb)



Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```

![8 o4 1](https://github.com/varshinidevaraju/Windows-basic-commands-batchscript/assets/144870750/49524d98-dc5f-4130-a085-58b47a3242cf)


![8 o4 2](https://github.com/varshinidevaraju/Windows-basic-commands-batchscript/assets/144870750/150bfdec-447f-4a7f-b254-385fd22a876c)




Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```

![8 o6](https://github.com/varshinidevaraju/Windows-basic-commands-batchscript/assets/144870750/b1051f2e-a4c4-4191-8bf0-4c54b5724ff8)



## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT
![8 o last](https://github.com/varshinidevaraju/Windows-basic-commands-batchscript/assets/144870750/a7560403-98df-4132-8226-0929c38e7537)


# RESULT:
The commands/batch files are executed successfully.


