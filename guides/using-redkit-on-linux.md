# Using REDkit on Linux

[Back to Home](../)



**This method was tested on Linux Mint v22.1 'Xia' Cinnamon Edition. This method is not guaranteed to work with other Linux distributions.**\
\
The Witcher 3 REDkit can run on Linux via Proton but can run into two common issues. Below are possible solutions

### Issue 1: Unable to find The Witcher 3 directory in Setup

This is due to steam being installed in a ".steam" folder, a hidden folder that the REDkit cannot see. To bypass this, we can create a symlink:\
\
1\. Create a new folder in your home directory and give it a name of your choosing e.g. steam\_symlink.\
2\. Find your steam folder (.steam/steam) and copy the full address. If you cannot find it, make sure that "Show Hidden Files" is ticked in the file manager.\
3\. Open up the console in your home directory and type `ln -s [Full path to your .steam/steam folder] [Folder you made]`. Do not include the square brackets in the command.\
4\. Check your symlink is working correctly by going into the folder you made and clicking on the file that should have appeared there. If it takes you to your steam folder then you have successfully created a symlink.\
5\. Open up the REDkit and when finding the Witcher 3 directory, navigate to the folder you made and click on the symlink. It should also take you to your steam folder and from there you can navigate to your Witcher 3 installation.

### Issue 2: Crashing while generating depot

This can depend on which version of Proton you are using. Using the latest experimental version appears to solve the issue.

### Known Issues

* Some user interface components can appear black or otherwise bugged visually. This is likely a symptom of the emulation process but it does not impact functionality. All tools work as intended.
