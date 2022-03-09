# Wall-for-Mac
Based on Spencr's and Jojoe's Wall, but made for Mac.

-----

Step One: Downloading

Keyboard Maestro - https://www.keyboardmaestro.com/main/

Twitch Studio - https://www.twitch.tv/broadcast/studio

Macros - https://github.com/BlenorTheGreat/Wall-for-Mac/releases (latest release here)

-----

Step Two: Configuration

Download Keyboard Maestro and grant it proper permissions. It should prompt you for these, but if not, go to System Preferences>Security&Privacy (click the lock in the bottom left corner to acess permissions) and grant permissions to both "Keboard Maestro" and "Keyboard Maestro Engine"

<img width="158" alt="Screen Shot 2022-03-09 at 4 04 42 PM" src="https://user-images.githubusercontent.com/99914793/157535842-1be814fa-fe28-4553-9700-c4684dabc337.png">
<img width="236" alt="Screen Shot 2022-03-09 at 4 05 05 PM" src="https://user-images.githubusercontent.com/99914793/157535897-c8acb2c5-b21b-4549-b473-c93349c6da53.png">

Then relaunch Keyboard Maestro. Next, open Terminal (do Command+Space and type "Terminal" to find it). Paste and run the following command:

<defaults write -g NSWindowResizeTime -float 0.003>

This will make it so instances will expand instantly instead of having to do the full MacOS animation (reduces time of the animation from 0.5s to 0.003s).
