# Lab Report 1 (Remote Connection):


## Installing VS Code
Download [VS Code](https://code.visualstudio.com/download) and openSSH if your PC doesn't have it. After that run the executable and choose your desired install path. Make sure you can open a new file under the file tab, and make note of your working directory (e.g., user\VSCode\projects). 
![VS Code Image](Step%20One%20Download%20VS%20Code.PNG)

## Remotely Connecting
In the Get Started menu of VS Code, click the Terminal buttom at the top left of the screen. In the drop-down menu, click the create new terminal button, and then from there type the following command to connect to your account: `ssh cs15lwi22XX@ieng6.ucsd.edu`, with XX being your assigned letters. You will then have to enter your password, and after that, you will be in the home directory of your student account.
![Remote Connection](Step%20Two.PNG)

## Trying Some Commands
Some example commands include `ls` to list all the files in your current directory, or `cd` followed by the directory name, to move to a directory within your current one. You can also use `cp` to copy files from a given directory, `make` to create new files, and when you're done, type `exit` to cut your connection.
![Example Commands](Step%20Three%20Example%20Commands.PNG)

## Moving Files with `scp`
Create a new java file like you normally would (i.e., click file, then hit new file), and from there do your coding. When you're ready to copy it to your server location open a new terminal like we did above in your file's working directory, then type in `scp "your file name" "your server name"` to copy it into your server account after you enter your password. You then close this terminal, and type `ls` in your home path in your server account terminal to ensure the file copied. After typing `ls`, you should observe your file in the list of files present, assuming you just copied it to the home directory of your terminal.
![StepFourPt1](StepFourOne.PNG)
![StepFourPt2](StepFourTwo.PNG)

## Setting an SSH key
Open a terminal in your user or PC directory, and then type in `ssh keygen`. Create a textfile in your user directory (i.e., utilize file explorer to navigate to the spot where you wish to store the key and create a blank text file) to store the key in it. Then, copy the directory in which you are working to the terminal where it asks for a file, and then enter a passphrase and store the key in that file. After that, boot up your student account, per the steps above, then type in `mkdir .ssh` to make a directory for your ssh key. Then use the `scp` command in the same terminal to copy the file with key from your user directory (see pic below) to your server account under the /.ssh/authorized_keys directory. You can navigate to your KeyGen directory using the `cd` commands in succession to move from directory to directory.

![StepFivePt1](StepFive.PNG)
![StepFivePt2](StepFiveTwo.PNG)

## Optimizing Remote Running
Talk about how many keystrokes the ssh key savesYou can run commands immediately after connecting via the same line in the terminal, or you can even run numerous files at once (Credit: Joe Politz).
![StepSix](BonusTips.PNG)
