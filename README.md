# Wall-for-Mac
*Based on Spencr's and Jojoe's Wall, but made for Mac.*

-----

## Step One: Downloading

- Keyboard Maestro - https://www.keyboardmaestro.com/main/
- Twitch Studio - https://www.twitch.tv/broadcast/studio
- Macros - https://github.com/BlenorTheGreat/Wall-for-Mac/releases/latest
- Positioning - https://www.spectacleapp.com/

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

Open Twitch Studio (it will ask you to sign in with your Twitch account). Create 5 scenes called "Wall Main" "Instance 1" "Instance 2" "Instance 3" "Instance 4" (Screen Share>Window NOT SCREEN)

![Screen Shot 2022-03-09 at 4 21 00 PM](https://user-images.githubusercontent.com/99914793/157538114-8442bc2e-07f2-4f56-95c4-9162ecb2867a.png)


Next, edit the "Wall Main" scene. Add the layers "Instance 1" "Instance 2" "Instance 3" "Instance 4" and a text layer on the top that indicates you're on the main screen (optional).

![Screen Shot 2022-03-09 at 4 34 15 PM](https://user-images.githubusercontent.com/99914793/157540029-a073c935-01b3-479c-8b8f-12b874764c5b.png)

------

## Step Four: Instance Setup

MultiMC is required for this macro. Make four instances and allocate 2048mb of RAM to each. Example:

<img width="428" alt="Screen Shot 2022-04-18 at 10 07 40 AM" src="https://user-images.githubusercontent.com/99914793/163819954-b317c5d8-e731-424b-bca3-bfe5475b1aff.png">

Use fabric for each (found in Edit Instance>Install Fabric) and performance mods found at https://www.minecraftspeedrunning.com (USE DYNAMIC MENU FPS). Launch each instance IN ORDER. I.E. Launch 1, wait for it to open. Launch 2, wait, etc. **DO NOT RESIZE THEM**. In your dock, they should be positioned in order. Now open Spectacle. Select instance one, and in your top bar, select "Upper Left"

<img width="229" alt="Screen Shot 2022-04-18 at 10 20 52 AM" src="https://user-images.githubusercontent.com/99914793/163821682-afd0866a-6fc9-4ac6-a261-a16af6c38609.png">

This should automatically resize it to fit your computer. Due to the mac's aspect ratio, it will also give you a slightly wider field of view, helpful for resetting.

In your "WALL MAIN" scene, go into each of your sources and select the corresponding instance. Move them to the same layout as they are on your screen. It should look like this:

![Screen Shot 2022-04-18 at 10 39 24 AM](https://user-images.githubusercontent.com/99914793/163824323-61f804d8-b067-410a-91a4-6b49867e7c27.png)

Let's clean this up. Click Instance 1, and select the crop tool. ![Screen Shot 2022-04-18 at 10 42 12 AM](https://user-images.githubusercontent.com/99914793/163824718-d89765fd-dce4-4645-bd22-873fe64a0f6e.png)

This is how your crop should look. ![Screen Shot 2022-04-18 at 10 42 31 AM](https://user-images.githubusercontent.com/99914793/163824771-2a4bd946-78ba-482a-b5bb-388774ce4520.png) Rinse and repeat for each instance.

![Screen Shot 2022-04-18 at 10 43 59 AM](https://user-images.githubusercontent.com/99914793/163825009-89d37ab4-dcbc-4f05-822b-b2273f2f9192.png)

Because of the wider field of view (which may vary by machine), there will be a space in the middle. Put whatever you want there or leave it blank. Alternativley, you can set the sizing mode to stretch and resize so that there is no gap.

![Screen Shot 2022-04-18 at 12 50 42 PM](https://user-images.githubusercontent.com/99914793/163842657-8c6c7675-85fd-4fa7-9faa-591a6a4e4dae.png)

![Screen Shot 2022-04-18 at 12 50 53 PM](https://user-images.githubusercontent.com/99914793/163842675-3ad2b3b4-ad6a-4af7-bb65-8a5a3b831aa8.png)

------

## Step Four: Configuring the Macros

There are 9 macros in total. 5 for resetting, 4 for playing.
