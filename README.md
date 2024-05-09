![326683013-f1f83410-e659-40ff-bee3-e079d93c7736](https://github.com/Dhanusha17/Windows-basic-commands-batchscript/assets/151549957/a70ee73b-c456-4de0-bffa-af6944a3bfde)# Windows-basic-commands-batchscript
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
```
mkdir %userprofile%\Desktop\MyLab
```
![326683013-f1f83410-e659-40ff-bee3-e079d93c7736](https://github.com/Dhanusha17/Windows-basic-commands-batchscript/assets/151549957/1b01332b-73df-45c5-8f44-6e763936d449)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![326683213-4de1b4bd-f842-485a-bf0d-90def6eaf1e9](https://github.com/Dhanusha17/Windows-basic-commands-batchscript/assets/151549957/bf11769f-9966-462a-8d65-bd155a7baacd)
![326683200-60ef83ad-950a-4bf7-ae70-7ccd4fae7aa7](https://github.com/Dhanusha17/Windows-basic-commands-batchscript/assets/151549957/6da069c7-abca-417c-a49c-df70301dfb8e)


## COMMAND AND OUTPUT
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![326683303-a28afee5-4fc8-4720-a29b-ae4c9819f177](https://github.com/Dhanusha17/Windows-basic-commands-batchscript/assets/151549957/d52acb5f-1d4e-4444-8fcd-ae1fd8bb2053)

## COMMAND AND OUTPUT
Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![326683342-ad0e4f9e-575b-48f5-95fe-7df3f52b5857](https://github.com/Dhanusha17/Windows-basic-commands-batchscript/assets/151549957/89870064-9d69-4f45-8a6f-fa8a5eae8512)

![326683348-fc1a73ef-f263-4896-9465-239e1420b390](https://github.com/Dhanusha17/Windows-basic-commands-batchscript/assets/151549957/f482084a-a449-4caa-8d1a-9e97afe09dad)


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![326683386-0fe73689-4d9b-4494-8ce8-d940fc9b9606](https://github.com/Dhanusha17/Windows-basic-commands-batchscript/assets/151549957/e1b157c0-ef11-44d0-9d5e-0492105ad266)

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
![326683409-f8257a6d-6fa4-4e1a-bc73-063fad3c5508](https://github.com/Dhanusha17/Windows-basic-commands-batchscript/assets/151549957/01925357-ba1f-4ea3-a0f9-69324d440a00)
## RESULT:
The commands/batch files are executed successfully.

