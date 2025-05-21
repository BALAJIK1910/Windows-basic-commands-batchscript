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
Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
mkdir %userprofile%\Desktop\MyLab
```

![1](https://github.com/user-attachments/assets/8e3d8348-7b08-4e01-823d-f7ff1d43b059)


## COMMAND AND OUTPUT
List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```


![2](https://github.com/user-attachments/assets/6ae4f35d-0c81-48c8-92ef-78677836cf2e)

![3](https://github.com/user-attachments/assets/cef88b2f-6d82-47ea-a36c-c13afeac527c)


## COMMAND AND OUTPUT
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```

![4](https://github.com/user-attachments/assets/a7f7e79f-3378-4ef5-a92d-e4651f0f27d0)


## COMMAND AND OUTPUT
Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```

![5](https://github.com/user-attachments/assets/667a777c-bdce-4a89-85eb-e964d7c46c3e)


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```

![6](https://github.com/user-attachments/assets/6d12bb24-a2ac-4f3c-99ce-e7f78a8e2e34)


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

![7](https://github.com/user-attachments/assets/888f4a8e-9bc2-4324-be9d-be36432f29a3)


# RESULT:
The commands/batch files are executed successfully.
