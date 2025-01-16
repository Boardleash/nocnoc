# nocnoc
![Alt text](./images/who.png)

Bash script to retrieve user related information on a Linux Host.

## Description

***nocnoc*** is a bash script intended to pull user related information on a Linux host.  This is an interactive script that will ask you if you wish to see this information.  You can simply answer "yes" or "no".  In either case, the response to your answer will be presented onto the terminal.  There are several hidden files created in order to store information for more processing.  At the end of script execution, these files are deleted from the system.  None of these files are intended to be saved (and are not due to the script).

The user information pulled consists of the following:

>	- *User executing the script*
>	- *Users that already exist on the host machine*
>	- *Currently logged in users*
>	- *Users who have accessed the host machine*
>	- *Users who attempted to access the host machine*

This script does not necessarily NEED to be ran with elevated privileges (root).  That said, if the script is ran without elevated privileges, you will not be able to retrieve information of the users who attempted to access the host machine.  If that information is desired, you should run this script with elevated privileges.

## Technologies Used

The script within the "**centos**" directory has been tested in the CentOS Stream 9 distribution, in both graphical and multi-user targets (GUI and Server).  The script within the "**ubuntu**" directory has been tested in the Ubuntu 24.04 LTS distribution, also in both graphical and multi-user targets.

The CentOS version of the script should also work with other similar flavors like Red Hat Enterprise Linux (RHEL), Fedora, Oracle, etc.

The Ubuntu version of the script should also work with similar Ubuntu flavors and Debian based distributions like Kali, Kubuntu, Parrot OS, etc.

## How To Download and Use

###### Method 1: Directly from my GitHub Repository

>	If not already in the repository, access it via the link below:
>		https://github.com/Boardleash/nocnoc/

>	Click on either "**centos**" or "**ubuntu**" (based on whichever OS you are using)

>	Click on the "**nocnoc**" file and then click on the download raw file option.

>	After the download is complete, go to where you downloaded the file.  The file will likely have been downloaded as a text file (.txt extension).  Rename the file to "**nocnoc**" (don't inlcude the .txt extension).

>	Right click the file and click on "**Properties**", then click on the "**Permissions**" tab.  Check the "**Allow executing file as program**" box.

>	After doing the above, you can right click on the file and select the "**Run as a program**" option.  The script will open a terminal session and execute.

###### Method 2: Via the Terminal

>	In your terminal, navigate to the directory that you wish to clone the repository into:
>	`cd <DIRECTORY TO CLONE REPO INTO>`

>	In the directory that you have just changed into, type the following:
>	> `git clone https://github.com/Boardleash/nocnoc/

>	This should successfully clone the entire **nocnoc** repository into the directory that you have chosen and you are now able to access the contents locally on your terminal

>	Navigate to where the "nocnoc" script is located.  By default this should be in `/PATH/TO/nocnoc/centos/` OR `/PATH/TO/nocnoc/ubuntu/,` but if this script was moved, then navigate to that appropriate directory.

>	Change file permissions for the script by typing the following:
>		*chmod 755 nocnoc*

>	Run the script by typing the following:
>		*./nocnoc*

>	The script will proceed.  It may take a minute, but once complete, you will be asked if you have gotten all that you need.  You can respond appropriately.
## ***NOTES***

>	- Be mindful of which OS you are using in order to execute the correct script
>	
>	- Acceptable forms of "yes" in this script are: 
>		- *Yes*
>		- *yes*
>		- *Y*
>		- *y*
>	
>	- Acceptable forms of "no" are:
>		- *No*
>		- *no*
>		- *N*
>		- *n*
