# Lab Report Week 6

## Streamlining SSH
First we need to access my SSH config file. To do this, we hit hit F1 and open a search bar in VS code, then type "ssh config" in the bar and click on the `Remote-SSH: Open SSH Configuration File`. This will open up the generic config file which has not been configured yet.![image](SSHConfigImage.png)

Now we edit the config file to our liking, as seen below, and create our alias `ieng6` using our account information. ![image](EditedUsingVSCode.PNG)

Assuming I have already completed the step from Lab One where I created an SSH key and made my computer an authorized user, all I have to do is type `ssh ieng6` to log into my account. 

![image](FirstWorks.PNG)

Even better, I can copy files using the `scp` command followed by the file I wish to copy followed by my alias `ieng6`, rather than typing my full account name everytime I wish to `ssh` into my account and copy a file. ![image](ItWorks.PNG)

As we can see, the file is there and the process worked!
