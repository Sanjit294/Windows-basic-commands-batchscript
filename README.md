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

![371380799-273cd6dc-d4e5-4894-8c8d-f348f3ba820a](https://github.com/user-attachments/assets/ecf0e5d8-323a-4461-959a-8874251bbf6e)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

cd %userprofile%\Desktop\MyLab

![371380873-98ba2b43-f1a8-45d7-9049-1493cbd5e86b](https://github.com/user-attachments/assets/a279c573-355c-4303-ae9d-aec5613db2b7)

![371380937-f7611b2b-5d55-405a-8c41-8886d57c866d](https://github.com/user-attachments/assets/cd98ee46-5288-43c0-84a8-4d39166b8726)



List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT

dir %userprofile%\Desktop\MyLab

![371381011-9c2e7a90-b4f1-443d-ac7e-d72405b94cf1](https://github.com/user-attachments/assets/62138837-8021-402b-a116-8dbaee5bbe2b)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![371381128-ca27f2a3-1bcb-45a4-8070-2612fccb62ec](https://github.com/user-attachments/assets/4a578ca9-4287-4b91-ac59-6e572090b759)

![371381217-c8eb6788-a1cf-4a83-bda3-ffb8997d71ae](https://github.com/user-attachments/assets/a221d13b-7638-43c5-be62-5ae727dd5e16)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
![371381319-6c53690b-653f-48e3-9a8e-0bb5dd204f09](https://github.com/user-attachments/assets/3704cff3-91b4-44dd-a119-e31083d22674)


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

![371381456-89d4a1ae-0207-40e3-b02c-6e03bd7d46d1](https://github.com/user-attachments/assets/be2c891b-1f8e-45f2-a86c-97c814135710)

# RESULT:
The commands/batch files are executed successfully.

