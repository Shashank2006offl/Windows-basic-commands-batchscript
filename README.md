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
~~~
mkdir %userprofile%\Desktop\MyLab
~~~
![329658320-0d1c931c-0132-467e-a239-1a645505b196](https://github.com/04Varsha/Windows-basic-commands-batchscript/assets/149035374/c65ec521-e638-4a1f-8bdd-97c56e1efc85)
Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
~~~
cd %userprofile%\Desktop\MyLab
~~~
![329659051-f2ae583f-91e3-49ac-bdcf-959749805451](https://github.com/04Varsha/Windows-basic-commands-batchscript/assets/149035374/b9be78f6-9828-4e71-a5a9-f6f1189783ed)
~~~
type nul > MyFile.txt
~~~
![329659348-6a8337f0-c88f-4b81-a611-16e5f0bec7f7](https://github.com/04Varsha/Windows-basic-commands-batchscript/assets/149035374/bd325e68-6b4b-4534-8545-4a27ff88884b)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
~~~
dir %userprofile%\Desktop\MyLab
~~~
![329659599-066144e3-43b8-4d7c-bf48-8a03d75d6c7e](https://github.com/04Varsha/Windows-basic-commands-batchscript/assets/149035374/30682b3a-8a3a-42f2-a0ce-4e01779085c9)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
~~~
mkdir %userprofile%\Desktop\Backup
~~~
![329659806-7a228e90-8940-43be-8231-4766db062bb7](https://github.com/04Varsha/Windows-basic-commands-batchscript/assets/149035374/64b3d1fb-6b15-47d7-b449-18d1df73456e)
~~~
copy MyFile.txt %userprofile%\Desktop\Backup
~~~
![329659991-e045c571-5703-455a-8d32-9aa6b2a2afde](https://github.com/04Varsha/Windows-basic-commands-batchscript/assets/149035374/6a48ce78-88e9-4a7e-a2e5-8ece42f7311e)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
~~~
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
~~~
![329660496-6b0dcb2a-0b98-4712-ac5a-4d558ca37037](https://github.com/04Varsha/Windows-basic-commands-batchscript/assets/149035374/1b3b3dfc-19ad-4574-98e2-e28bd46533f1)




## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
## COMMAND:
~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
~~~
![329660834-0594a6df-84d8-4328-a347-5e6ca215a41c](https://github.com/04Varsha/Windows-basic-commands-batchscript/assets/149035374/759f68b0-4717-4bea-9e37-4f8bc436e3b6)
## COMMAND:
~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
~~~
## OUTPUT
![329661256-27953f04-f5d1-4b1f-a369-60b6cb1d90e1](https://github.com/04Varsha/Windows-basic-commands-batchscript/assets/149035374/c3bd3e5a-2d4b-4db4-b681-8557bc05d5c6)

## RESULT:
The commands/batch files are executed successfully.






# RESULT:
The commands/batch files are executed successfully.

