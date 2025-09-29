# Guide to Set Up STALKER IWP on Linux

## Setting Up Flatpak and Bottles

1. Before we begin, we need to verify that the distribution you have selected supports Flatpak.

2. Use this link to verify that the distribution you have selected supports Flatpak:
   https://flatpak.org/setup/

   2a. If your distribution does not have Flatpak installed, follow the guide provided to get set up.

   2b. To verify that you have installed correctly, open your terminal (Ctrl+T) and type in the following command:

         flatpak --version
   
   2c. Currently, v1.16.0 is the latest build of Flatpak.

4. Now that you have verified that Flatpak is installed, you can go to your distribution’s software center and search “Bottles”

5. Install Bottles.

6. Before opening Bottles enter this command into your terminal so you can give permission to bottles to access your file system

        sudo flatpak override --user --filesystem=host com.usebottles.bottles

8. Open Bottles and go through the initial set up.

9. Once the initial set up is complete, in the top-left click the three-dot icon in the top-right of Bottles, then select “Preferences”

10. Go to “Runners” At the bottom you should see "Proton GE".

11. Click “Download & Install” to install Proton 10-17.

    8a. As of the time of writing this , the latest Proton build is 10-17.

12. In the top-left of Bottles, click the “+” icon to create a new bottle.

13. Name this bottle “Games” as you can use this for more games than just IWP.


## Setting Up the Bottle

14. Open the "Games" bottle.

15. You should see the following availible to you "Programs", "Options", and "Tools".

16. Under “Options” click "Settings".

17. You should see "Components". Under "Components" you should see "Runner" to verify that it is "ge-proton10-17".

18. Close the settings menu.


## Installing STALKER IWP

19. Download the IWP from the following MODDB link:
    https://www.moddb.com/mods/stalker-improved-weapon-pack/downloads/iwp-standalone

20. Download IWP Second Patch from the following MDDB link:
    https://www.moddb.com/mods/stalker-improved-weapon-pack/downloads/patch-for-standalone

21. Extract IWP first into the directory you desire for example "mnt/SDD1/Games/IWP".

22.  Extract the Second Patch files into the IWP directory and allow any overwrites to all files within the directory.

     22a. You will notice the verbage is different from Windows slightly however the process is the same depending on your file manager your distro uses. Check with your distro's wiki page to verify what it uses as a file manager.

## Back to Bottles

23.  Within Bottles click on your "Games" bottle.

24.  Once you are there you should see the following "Programs", "Options", and "Tools".

25.  Under "Programs" click "Add Shortcuts".

26.  Point Bottles to where ever you have installed IWP to find "Launcher.exe" for me it's "/mnt/SSD1/Games/IWP/Launcher.exe".

      26a.You can repeat these previous four steps above to add the JSGME.exe mod manager and run mods the same as you would Windows

27.  Once you have selected the executable successfully you should see it added under "programs" as "Launcher".

28.  From here you can click play.

       28a. Next to the play button there is a three dots icon that allows you to set your launch options. I would recommened to click "Add to Steam". This will allow it to launch through Steam as a standard game in your library. You will need to restart Steam for it to appear.

29.  Congratulations you have setup IWP to work on Linux.


## Troubleshooting

1. If the game does not start, double-check that the correct Proton GE runner is selected.

2. If you still encounter issues, try creating afresh bottle. Then add the Launcher.exe.

3. You can also check the official Bottles documentation for further troubleshooting.
