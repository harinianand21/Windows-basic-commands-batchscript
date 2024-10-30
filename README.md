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
![328876486-e82e2f99-bead-4ce0-a456-acc495de960e](https://github.com/amirthaviswanathan05/Windows-basic-commands-batchscript/assets/149035397/e3b2d0f6-c986-4c88-8f81-ec378a2265dc)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![328876538-072bf08b-8f1f-47e7-9ce0-4bd5389e5e43](https://github.com/amirthaviswanathan05/Windows-basic-commands-batchscript/assets/149035397/244486d7-d57a-4160-b4a4-71152c83cc76)
```
type nul > MyFile.txt
```
![328876592-72daf233-97b8-4bab-829b-4e43929a4fb1](https://github.com/amirthaviswanathan05/Windows-basic-commands-batchscript/assets/149035397/3229aa5d-47bc-4ece-8b48-eb76f933308a)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![328876668-ffa2b94b-cc47-478d-aaaf-e07201189f9f](https://github.com/amirthaviswanathan05/Windows-basic-commands-batchscript/assets/149035397/2e5927c2-9502-4128-8867-f4331ece1cb0)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![328876764-b398f90e-ae0b-4acd-9f4c-f61ecfe8cb82](https://github.com/amirthaviswanathan05/Windows-basic-commands-batchscript/assets/149035397/98b6f15e-1caa-420d-818b-6ad46a1a75fa)
```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![328876840-98ab3063-d62a-4eb1-96a3-444a8d8aff5d](https://github.com/amirthaviswanathan05/Windows-basic-commands-batchscript/assets/149035397/62203b81-3e36-4d45-9d0e-10025cac9514)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents

move MyLab Documents
```
![328877293-342ac881-4ac9-4c2f-a6a0-cdc37248f16c](https://github.com/amirthaviswanathan05/Windows-basic-commands-batchscript/assets/149035397/be95ee3b-87df-4d67-97e7-7af608b91222)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

# COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

## OUTPUT

![328876946-c6377772-a55f-4d77-9d2c-78ea30ece3d9](https://github.com/amirthaviswanathan05/Windows-basic-commands-batchscript/assets/149035397/4773565c-b5a4-434e-a7dc-52817697eff0)

# COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
![328877014-777c22b5-a3b1-444f-ad7a-045c05cd0d9c](https://github.com/amirthaviswanathan05/Windows-basic-commands-batchscript/assets/149035397/d7e77e7f-05ef-4e45-bb32-2e4df33c98f2)

# RESULT:
The commands/batch files are executed successfully.
