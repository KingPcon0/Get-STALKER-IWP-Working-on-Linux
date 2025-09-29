# Guide to Set Up STALKER IWP on Linux

## Setting Up Flatpak and Bottles

1. Before we begin, we need to verify that the distribution you have selected supports Flatpak.

2. Use this link to verify that the distribution you have selected supports Flatpak:
   https://flatpak.org/setup/

   a. If your distribution does not have Flatpak installed, follow the guide provided to get set up.

   b. To verify that you have installed Flatpak correctly. Open your terminal (Ctrl+T) and type in the following command:

         flatpak --version
   
   c. The latest build of Flatpak currently v1.16.0 is.

4. Now that you have verified that Flatpak is installed, you can go to your Linux distribution’s software center and search “Bottles”

5. Install Bottles.
   a. You can also install via the terminal if prefered flathub.org link here:
   

6. Before opening Bottles enter this command into your terminal so you can give permission to Bottles to access your file system

        sudo flatpak override --user --filesystem=host com.usebottles.bottles

8. Open Bottles and go through the initial set up.

9. Once the initial set up is complete, in the top-right click the three-dot icon in Bottles, then in the drop down menu select “Preferences”.

10. Go to the “Runners” tab at the top within the "Prefernces" window, then towards the bottom and you should see "Proton GE". 

11. Click “Download & Install” to install Proton 10-17.

    a. At the time of writing this, the latest Proton build is 10-17.

12. In the top-left of Bottles, click the “+” icon to create a new bottle.

13. Name this bottle “Games” as you can use this for more games than just IWP.

14. Select the "Gaming" option when creating a fresh bottle, then in the "Runners" drop down select "ge-proton10-17"



## Setting Up the Bottle

15. Click the "Games" bottle you have just created.

16. You should see the following availible to you "Programs", "Options", and "Tools".

17. Under “Options” click "Settings".

18. You should see "Components". Under "Components" you should see "Runner" to verify that it is "ge-proton10-17" is selected.

19. Close the settings menu.


## Installing STALKER IWP

20. Download the IWP from the following MODDB link:
    https://www.moddb.com/mods/stalker-improved-weapon-pack/downloads/iwp-standalone

21. Download IWP Second Patch from the following MDDB link:
    https://www.moddb.com/mods/stalker-improved-weapon-pack/downloads/patch-for-standalone

22. Extract IWP first into the directory you desire for example "mnt/SDD1/Games/IWP".

23. Extract the Second Patch files into the IWP directory and allow any overwrites to all files within the directory.

     a. You will notice the verbage is different from Windows slightly however the process is the same depending on your file manager your distro uses. Check with your distro's wiki page to verify what it uses as a file manager.

## Back to Bottles

24.  Within Bottles click on your "Games" bottle.

25.  Once you are there you should see the following "Programs", "Options", and "Tools".

26.  Under "Programs" click "Add Shortcuts".

27.  Point Bottles in the direction of where ever you have installed IWP to find "Launcher.exe" for example it's "/mnt/SSD1/Games/IWP/Launcher.exe".

   a. You can repeat steps 24-27 above to add the JSGME.exe mod manager and run mods the same as you would Windows
    
   b. You can also run Mod Organizer 2 as well just repeat steps 24-27 to add ModOrganizer.exe if you use MO2 for managing your mods

28. Once you have selected the executable successfully you should see it added under "programs" as "Launcher".

   a. You can rename "Launcher" to IWP by looking at the three-dot icon to the right of "Launcher" within the drop down menu you should see "Rename"
   
   b. If you decide to rename it you will need to remove it from steam and re-add it again by repeating step 29a

29. From here you can click play.

   a. If you want to add this to Steam. You will notice next to the play button there is a three dots icon that allows you to set your launch options. From the drop down menu you will see "Add to Steam". This will allow it to launch through Steam as a standard game in your library. You will need to restart Steam for it to appear.

30. Congratulations you have setup IWP to work on Linux.


## Troubleshooting

1. If the game does not start, double-check that the correct Proton GE runner is selected.

2. If you still encounter issues, try creating afresh bottle. Then add the Launcher.exe.

3. You can also check the official Bottles documentation for further troubleshooting.
