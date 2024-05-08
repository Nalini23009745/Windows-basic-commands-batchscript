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
mkdir %userprofile%\Desktop\MyLab
![image](https://github.com/Nalini23009745/Windows-basic-commands-batchscript/assets/149347484/0ccaae11-06d7-43a4-8fa0-6e3250ad1ebb)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![image](https://github.com/Nalini23009745/Windows-basic-commands-batchscript/assets/149347484/783930bf-10aa-4ff1-917c-5d20f43a79bb)
![image](https://github.com/Nalini23009745/Windows-basic-commands-batchscript/assets/149347484/2680caac-3ad6-4c2a-bf00-b0e341d40d7e)



List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab
![image](https://github.com/Nalini23009745/Windows-basic-commands-batchscript/assets/149347484/cbdc6990-1ce4-414d-acf2-8c8252a13c12)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
![image](https://github.com/Nalini23009745/Windows-basic-commands-batchscript/assets/149347484/dafda859-55ae-4269-b184-3b0aa684fb99)
![image](https://github.com/Nalini23009745/Windows-basic-commands-batchscript/assets/149347484/e5678769-6fbb-4b26-a950-2df21e664268)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents
![image](https://github.com/Nalini23009745/Windows-basic-commands-batchscript/assets/149347484/d1752880-a3ed-4306-8956-47ef3fb3944a)


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
![image](https://github.com/Nalini23009745/Windows-basic-commands-batchscript/assets/149347484/097fd8da-2eb8-4d2a-87f6-8fbd438a8ced)





# RESULT:
The commands/batch files are executed successfully.

