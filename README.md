# Stephen O Neill C13317851
## Systems integration Assignment 1
## Custom Shell
### Outline
Assignment 1 enlisted us to create a custom shell for a specified user on a linux system
The purpose of a custom shell is to allow the specified user limited access to certain 
commands and locations on the system which can simplify the system for said user to use.
This was what i have set out to accompplish with my code

### Instructions for download
#### NOTE: you must be super user to run command : sudo su or just sudo before any command then enter your password

1.Download this repo to your system using this command in your terminal

  git clone https://github.com/szteve/sysassignment

2.cd into the repo using: cd sysassignment

3.Compile the code using 

  sudo chmod 775 backup NOTE: must have password for sudo to work

4.Now the shell is on youre system you must specify it to the user

### User 
If a user for the shell doesnt exist then you must create one

1.To create user use commmand :  useradd -m username
2.Now you must set a password for the user using command : passwd

Now that the user is created we can move on to specifying the shell for the user

1.To point the user to the shell we use the command usermod as such

         usermod -s directoryname/sysassignment/shelly username
         
After running this command the user will be specified to the shell
Now when the user logs in all they will see is the custom shell

### User Login

1.To switch to the desired user you can use the command
      
      su username
