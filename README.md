# Update OpenCore to the latest version
Update OpenCore (and EFI) to latest version using OpenCore Configurator

![alt test](/Pictures/OpenCoreUpdate.png)

# Introduction
Many of you asking how do I upgrade my OpenCore to the latest version. Updating OpenCore is not so easy as i.e. updating Clover, so therefore I made myself a small how-to to make lives easier. Hopefully this is of value to you.

Steps I undertake to upgrade OpenCore to the latest (stable) released build (it now takes me 30 minutes to do this per system): 

[<img src="/Pictures/Youtube-Thumbnail-joost.png" width="50%">](https://www.youtube.com/watch?v=332c2HnPvoU "Update OpenCore")

# 1. Check your current OpenCore version
Open Terminal app, and enter (without brackets) 
" nvram 4D1FDA02-38C7-4A6A-9CC6-4BCCA8B30102:opencore-version " 
and check which version of OpenCore you're currently using.
 
 ![alt test](/Pictures/2022-07-04_09-03-42.png)


# 2. Check the Dortania website
This is important for you to understand the changes in OpenCore. Dortania made a small how-to:
https://dortania.github.io/OpenCore-Post-Install/universal/update.html
And the Differences comparison can be handy:
https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Differences/Differences.pdf

The thing I find not so usefull here, is that you need to understand everything in the document, which is not so good for the more beginning hackintoshers (like myself). So, therefore, I follow my own little procedure as per below. 

# 3.1 Upgrade with OCAuxiliaryTools.app
My preferred option is to use OCAuxiliaryTools.app ( https://github.com/ic005k/OCAuxiliaryTools )

Open the application.
 ![alt test](/Pictures/1-OCupdate.png)

Press Edit in the menu-bar and chose for OpenCore DEV to get the latest OC version in development (can be handy for the latest macOS version support). Then, in the same menu, choose 'Mount ESP' (which is your EFI) and load config.plist. 

 ![alt test](/Pictures/3-OCupdate.png)

 You will probably see the red icon. You can ignore that, it's just saying that your current database version is not suitable for your EFI version. 
 ![alt test](/Pictures/4-OCupdate.png)

Press the Update icon 'Upgrade OpenCore and Kexts
 ![alt test](/Pictures/2-OCupdate.png)

Select All kexts and Update them.
 ![alt test](/Pictures/6-OCupdate.png)

Then select all OpenCore files and press 'Get OpenCore' 
 ![alt test](/Pictures/5-OCupdate.png)
 ![alt test](/Pictures/7-OCupdate.png)

 Press OK
 ![alt test](/Pictures/8-OCupdate.png)

 and then press 'Start Sync'
 ![alt test](/Pictures/9-OCupdate.png)

Press OK
 ![alt test](/Pictures/10-OCupdate.png)

Press on File in the Menu-bar and press Save. Your EFI is now saved and OpenCore is updated! 
 ![alt test](/Pictures/11-OCupdate.png)

 
# 3.2 Upgrade with HackinDROM

This video shows you how to download, install and configure the HackinDROM app, ultimately to update OpenCore in a very easy and convenient manner.

Credits to HackinDROM developer 'Inqnuam' and tester/guide writer 'CaseySJ' over at https://www.tonymacx86.com/

https://www.youtube.com/watch?v=xRuerrG-lAU

Download HackinDROM here: https://github.com/Inqnuam/HackinDROM

