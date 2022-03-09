# Wall-for-Mac
*Based on Spencr's and Jojoe's Wall, but made for Mac.*

-----

## Step One: Downloading

- Keyboard Maestro - https://www.keyboardmaestro.com/main/
- Twitch Studio - https://www.twitch.tv/broadcast/studio
- Macros - https://github.com/BlenorTheGreat/Wall-for-Mac/releases/latest

-----

## Step Two: Keyboard Maestro Configuration

Open Keyboard Maestro and grant it proper permissions. It should prompt you for these, but if not, go to
```
System Preferences > Security & Privacy > Click the lock in the bottom left corner to access permissions
```
And grant permissions to both "Keboard Maestro" and "Keyboard Maestro Engine"

<img width="158" alt="Image" src="https://user-images.githubusercontent.com/99914793/157535842-1be814fa-fe28-4553-9700-c4684dabc337.png">
<img width="236" alt="Image" src="https://user-images.githubusercontent.com/99914793/157535897-c8acb2c5-b21b-4549-b473-c93349c6da53.png">

Paste and run the following command in Terminal:
```
defaults write -g NSWindowResizeTime -float 0.003
```

------

## Step Three: Twitch Studio Configuration

Open Twitch Studio (it will ask you to sign in with your Twitch account). Create 5 scenes called "Wall Main" "Instance 1" "Instance 2" "Instance 3" "Instance 4" 

![Screen Shot 2022-03-09 at 4 21 00 PM](https://user-images.githubusercontent.com/99914793/157538114-8442bc2e-07f2-4f56-95c4-9162ecb2867a.png)


Next, edit the "Wall Main" scene. Add the layers "Instance 1" "Instance 2" "Instance 3" "Instance 4"
