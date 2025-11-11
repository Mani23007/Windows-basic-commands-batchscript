# Windows-basic-commands-batchscript
## Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file . Save each script in a file with a .bat extension. Ensure you have the necessary permissions to perform the operations. Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations

### Create a directory named "my-folder"

## COMMAND AND OUTPUT:

<img width="615" height="96" alt="1 output" src="https://github.com/user-attachments/assets/70b2ec31-8557-4c1d-8578-3e14db9f4155" />

### Remove the directory "my-folder"

## COMMAND AND OUTPUT:
<img width="602" height="86" alt="2 output" src="https://github.com/user-attachments/assets/a75e4db6-f16e-479b-90e1-0d068e8f50a5" />



### Create the file Rose.txt

## COMMAND AND OUTPUT:

<img width="698" height="82" alt="3 output" src="https://github.com/user-attachments/assets/b18d191f-c0fa-46ac-8d9b-d57d8fa0b041" />


### Create the file hello.txt using echo and redirection

## COMMAND AND OUTPUT:

<img width="815" height="86" alt="4 output" src="https://github.com/user-attachments/assets/04a242c7-7dab-47f5-af81-e1523fb55ac6" />


### Copy the file hello.txt into the file hello1.txt

## COMMAND AND OUTPUT:

<img width="795" height="107" alt="5 output" src="https://github.com/user-attachments/assets/4d90381c-8275-43c8-bed6-e0d18172968f" />


### Remove the file hello1.txt

## COMMAND AND OUTPUT:

<img width="652" height="86" alt="output 6" src="https://github.com/user-attachments/assets/6903d0f0-d666-4f17-b43d-b205a176b60b" />

### List out the file hello1.txt in the current directory

## COMMAND AND OUTPUT:

<img width="635" height="185" alt="output 7" src="https://github.com/user-attachments/assets/d0246ce2-31dc-43c6-ac19-c6d0c98062f3" />

### List out all the associated file extensions 

## COMMAND AND OUTPUT:

<img width="608" height="872" alt="output 8" src="https://github.com/user-attachments/assets/2240aa4d-d26e-45f7-a37a-929c948030ce" />


### Compare the file hello.txt and rose.txt

## COMMAND AND OUTPUT:
<img width="607" height="191" alt="output 9" src="https://github.com/user-attachments/assets/e3a86ef2-27b2-4b69-9315-be0117cbb737" />


## Exercise 2: Advanced Batch Scripting
Create a batch file named on the desktop. The batch file need to have a variable assigned with a desired name for ex. name="John" and display as "Hello, John".

## OUTPUT:
<img width="452" height="102" alt="output 10" src="https://github.com/user-attachments/assets/f982557a-86e6-4e82-8296-4406ae50a760" />




Create a batch file  on the desktop that checks whether a user-input number is odd or not. The script should:
Prompt the user to enter a number.
Calculate the remainder when the number is divided by 2.
Display whether the number is odd or not.
Ask the user if they want to check another number.
Repeat the process if the user enters Y, and exit with a thank-you message if the user enters N.
Handle invalid inputs for the continuation prompt (Y/N) gracefully.



## OUTPUT:

<img width="482" height="218" alt="output 11" src="https://github.com/user-attachments/assets/f05efedf-2111-4964-8bdc-c6eb1def717a" />




Write a batch file that uses a FOR loop to iterate over a sequence of numbers (1 to 5) and displays each number with the label Number:. The output should pause at the end.




## OUTPUT:

<img width="493" height="183" alt="output 12" src="https://github.com/user-attachments/assets/7f833a2c-309c-41e6-a677-3c393389c8b4" />




Write a batch script to check whether a file named sample.txt exists in the current directory. If the file exists, display the message sample.txt exists. Otherwise, display sample.txt does not exist. Pause the script at the end to view the result.

Instructions:
Use the IF EXIST conditional statement.
Make sure the script works for files located in the same directory as the batch file.
Use pause to keep the command window open after displaying the message.
Expected Output (if the file exists):

## OUTPUT:
<img width="503" height="112" alt="output 13" src="https://github.com/user-attachments/assets/730d8e3c-09b0-432e-a537-65f566a9d3a1" />



Write a batch script that displays a simple menu with three options:
Say Hello – Displays the message Hello, World!
Create a File – Creates a file named newfile.txt with the content This is a new file
Exit – Exits the script with a goodbye message
The script should repeatedly display the menu until the user chooses to exit. Use goto statements to handle menu navigation.


## OUTPUT:
<img width="352" height="142" alt="output 14" src="https://github.com/user-attachments/assets/f74cd329-8ca9-4da7-94c5-fd60233273eb" />
<img width="352" height="136" alt="output 15" src="https://github.com/user-attachments/assets/82d77782-acac-4f05-8d4b-df4a5d2f76fc" /> 
<img width="357" height="142" alt="output 16" src="https://github.com/user-attachments/assets/ab22c265-b937-4ecb-b7ec-670d73d401c2" />


# RESULT:
The commands/batch files are executed successfully.

