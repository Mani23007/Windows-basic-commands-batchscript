# Windows-basic-commands-batchscript
## Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

- Write the Windows commands / batch file .
- Save each script in a file with a .bat extension.
- Ensure you have the necessary permissions to perform the operations. Adapt paths as needed based on your system configuration.
### Step 3:

- Execute the necessary commands/batch file for the desired output. 

# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
### Create a directory named "my-folder"

## COMMAND AND OUTPUT:

<img width="615" height="96" alt="1 output" src="https://github.com/user-attachments/assets/b222baa2-6e10-4f57-b9dd-bfccafa8dd53" />


### Remove the directory "my-folder"

## COMMAND AND OUTPUT:

<img width="602" height="86" alt="2 output" src="https://github.com/user-attachments/assets/0116a52b-cf79-4e48-9d8c-787662a1c9f4" />

### Create the file Rose.txt

## COMMAND AND OUTPUT:

<img width="698" height="82" alt="3 output" src="https://github.com/user-attachments/assets/5f6e5c55-66cd-4bdd-aad2-41d312a614cf" />

### Create the file hello.txt using echo and redirection

## COMMAND AND OUTPUT:

<img width="815" height="86" alt="4 output" src="https://github.com/user-attachments/assets/26f1c137-b522-44ec-8d33-6d67b72bf0f5" />

### Copy the file hello.txt into the file hello1.txt

## COMMAND AND OUTPUT:

<img width="795" height="107" alt="5 output" src="https://github.com/user-attachments/assets/c13a36c2-41dd-4bb7-a959-36e5c19801c2" />

### Remove the file hello1.txt

## COMMAND AND OUTPUT:

<img width="652" height="86" alt="output 6" src="https://github.com/user-attachments/assets/52a043e5-d446-4cc1-ac1e-3d9b93e1b84b" />

### List out the file hello1.txt in the current directory

## COMMAND AND OUTPUT:

<img width="635" height="185" alt="output 7" src="https://github.com/user-attachments/assets/0c58e712-5ad5-4d9b-9e68-f0ace4c3dbd9" />

### List out all the associated file extensions 

## COMMAND AND OUTPUT:

<img width="608" height="872" alt="output 8" src="https://github.com/user-attachments/assets/811c3467-8102-49ba-9d0c-151d9dba575c" />


### Compare the file hello.txt and rose.txt

## COMMAND AND OUTPUT:

<img width="607" height="191" alt="output 9" src="https://github.com/user-attachments/assets/32a2cafe-3488-48f7-8ea9-59dcad96c4c9" />

## Exercise 2: Advanced Batch Scripting
1.Create a batch file named on the desktop. The batch file need to have a variable assigned with a desired name for ex. name="John" and display as "Hello, John".

## BATCH PROGRAM:

```bat
@echo off
set name=John
echo Hello, %name%
pause
```

## OUTPUT:

<img width="452" height="102" alt="output 10" src="https://github.com/user-attachments/assets/7b32429e-159e-4103-8882-02902e858f2e" />


2.Create a batch file  on the desktop that checks whether a user-input number is odd or not. The script should:
- Prompt the user to enter a number.
- Calculate the remainder when the number is divided by 2.
- Display whether the number is odd or not.
- Ask the user if they want to check another number.
- Repeat the process if the user enters Y, and exit with a thank-you message if the user enters N.
- Handle invalid inputs for the continuation prompt (Y/N) gracefully.

## BATCH PROGRAM:
```bat
@echo off
:loop
set /p num=Enter a number: 
set /a rem=%num% %% 2

if %rem%==0 (
    echo %num% is Even
) else (
    echo %num% is Odd
)

:ask
set /p ans=Do you want to check another number? (Y/N): 
if /I "%ans%"=="Y" goto loop
if /I "%ans%"=="N" goto end
echo Invalid input. Please enter Y or N.
goto ask

:end
echo Thank you!
pause
```

## OUTPUT:

<img width="482" height="218" alt="output 11" src="https://github.com/user-attachments/assets/8a1b414f-e15e-4893-a4c8-ca392113612c" />

3.Write a batch file that uses a FOR loop to iterate over a sequence of numbers (1 to 5) and displays each number with the label Number:. The output should pause at the end.

## BATCH PROGRAM:
```bat
@echo off
for /L %%i in (1,1,5) do (
    echo Number: %%i
)
pause
```
## OUTPUT:

<img width="493" height="183" alt="output 12" src="https://github.com/user-attachments/assets/e618269e-deb1-42dc-b4d1-f6f14ad0c3f7" />




4.Write a batch script to check whether a file named sample.txt exists in the current directory. If the file exists, display the message sample.txt exists. Otherwise, display sample.txt does not exist. Pause the script at the end to view the result.

Instructions:
- Use the IF EXIST conditional statement.
- Make sure the script works for files located in the same directory as the batch file.
- Use pause to keep the command window open after displaying the message.
- Expected Output (if the file exists):

## BATCH PROGRAM:
```bat
@echo off
if exist sample.txt (
    echo sample.txt exists.
) else (
    echo sample.txt does not exist.
)
pause
```

## OUTPUT:

<img width="503" height="112" alt="output 13" src="https://github.com/user-attachments/assets/356989f5-053b-4bf2-b755-743b6111fc45" />

5.Write a batch script that displays a simple menu with three options:
- Say Hello – Displays the message Hello, World!
- Create a File – Creates a file named newfile.txt with the content This is a new file
- Exit – Exits the script with a goodbye message
- The script should repeatedly display the menu until the user chooses to exit. Use goto statements to handle menu navigation.

## BATCH PROGRAM:
```bat
@echo off
:menu
cls
echo 1. Say Hello
echo 2. Create a File
echo 3. Exit
set /p choice=Choose an option (1-3): 

if "%choice%"=="1" goto hello
if "%choice%"=="2" goto create
if "%choice%"=="3" goto exit
echo Invalid choice.
pause
goto menu

:hello
echo Hello, World!
pause
goto menu

:create
echo This is a new file > newfile.txt
echo File newfile.txt created.
pause
goto menu

:exit
echo Goodbye!
pause
exit
```

## OUTPUT:

<img width="352" height="142" alt="output 14" src="https://github.com/user-attachments/assets/51b2070f-9db6-477a-902b-b0037edd0ac1" />

<img width="352" height="136" alt="output 15" src="https://github.com/user-attachments/assets/8842a5fc-f33d-47f3-b3ce-8f99f9c27047" />

<img width="357" height="142" alt="output 16" src="https://github.com/user-attachments/assets/bbc008d3-b22f-4968-899d-670c9d9a0eb8" />

# RESULT:
The commands/batch files are executed successfully.

