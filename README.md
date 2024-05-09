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
![image](https://github.com/rdxkeerthi/Windows-basic-commands-batchscript/assets/147473120/e995f79f-aaba-442c-9656-a2a08254ae6e)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![image](https://github.com/rdxkeerthi/Windows-basic-commands-batchscript/assets/147473120/42716050-4c57-409a-ba15-bc74916e236b)
![image](https://github.com/rdxkeerthi/Windows-basic-commands-batchscript/assets/147473120/5261ae76-6da8-4099-af43-454d30a7bb0c)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLa
![image](https://github.com/rdxkeerthi/Windows-basic-commands-batchscript/assets/147473120/a75e0d20-0ba6-4908-9719-1e2b13aea1d4)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
![image](https://github.com/rdxkeerthi/Windows-basic-commands-batchscript/assets/147473120/cb5e75d6-e7c9-4b0f-a0c1-89b066b228f6)
![image](https://github.com/rdxkeerthi/Windows-basic-commands-batchscript/assets/147473120/526cd0df-ca0c-41cf-b4c1-555cd69d29dc)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents
![image](https://github.com/rdxkeerthi/Windows-basic-commands-batchscript/assets/147473120/703084f3-b524-4ed7-bb9c-c6fba705eb95)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```




## OUTPUT
![image](https://github.com/rdxkeerthi/Windows-basic-commands-batchscript/assets/147473120/469a4295-b9e1-44b5-9c40-ed949f8fb79e)





# RESULT:
The commands/batch files are executed successfully.

