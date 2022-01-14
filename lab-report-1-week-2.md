Lab Report 1 (Remote Connection):

![VS Code Image](Step%20One%20Download%20VS%20Code.PNG)
Step One: Download [VS Code](https://code.visualstudio.com/download). After that run the executable and choose your desired install path. Make sure you can open a new file etc.

![Remote Connection](Step%20Two.PNG)
Step Two: In the Get Started menu of VS Code, click the Terminal buttom at the top left of the screen. In the drop-down menu, click the create new terminal button, and then from there type the following command to connect to your account: ssh cs15lwi22ajx@ieng6.ucsd.edu

![Example Commands](Step%20Three%20Example%20Commands.PNG)
Step Three: You should see something similar to the picture above. Now play around with some example commands like ls to list all the files in your current directory, or cd to move to directory within your current one.

![StepFourPt1](StepFourOne.PNG)
![StepFourPt2](StepFourTwo.PNG)
Step Four: Create a new java file like you normally would (i.e., new file), and from there do your coding. When you're ready to copy it to your server location open a new terminal in your file's working directory, then type in scp "your file name" "your server name" to copy it into your server account after you enter your password. You then close this terminal, and type ls in your home path in your server account terminal to ensure the file copied.

