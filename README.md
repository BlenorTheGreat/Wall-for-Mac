# Wall-for-Mac
*Based on Spencr's and Jojoe's Wall, but made for Mac.*

-----

## Step One: Downloading

- Keyboard Maestro - https://www.keyboardmaestro.com/main/
- Twitch Studio - https://www.twitch.tv/broadcast/studio
- Macros - https://github.com/BlenorTheGreat/Wall-for-Mac/releases/latest
- Spectacle - https://www.spectacleapp.com/

-----

## Step Two: Keyboard Maestro Configuration

Open Keyboard Maestro and grant it proper permissions. It should prompt you for these, but if not, go to
```
System Preferences > Security & Privacy > Click the lock in the bottom left corner to access permissions
```
And grant permissions to both "Keboard Maestro" and "Keyboard Maestro Engine"

<img width="158" alt="Image" src="https://user-images.githubusercontent.com/99914793/157535842-1be814fa-fe28-4553-9700-c4684dabc337.png">
<img width="236" alt="Image" src="https://user-images.githubusercontent.com/99914793/157535897-c8acb2c5-b21b-4549-b473-c93349c6da53.png">

Restart Keyboard Maestro.

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

Edit each Instance scene, and create a text layer and screen share. Set the screenshare to your full screen, but crop out the top bar (![Screen Shot 2022-04-18 at 3 28 06 PM](https://user-images.githubusercontent.com/99914793/163864940-19ad8697-3739-4bd4-8271-9b60b94b8503.png)
) and dock like so:

![Screen Shot 2022-04-18 at 3 27 25 PM](https://user-images.githubusercontent.com/99914793/163864861-884b31bf-9106-4e45-b0a9-52a420613054.png)

Text layer should say #1. Repeat for each instance.

Go to the hotkey screen in settings, and set your hotkeys to the following:

![Screen Shot 2022-04-18 at 2 53 09 PM](https://user-images.githubusercontent.com/99914793/163859865-aad80537-7f49-4cc4-b1b1-5917dd3ae644.png)


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

There are 9 macros in total. 5 for resetting, 4 for playing. Let's begin with the switching macros. Select "Switch to Instance 1" (if this is your first boot of Keyboard Maestro, you might have to click edit at the bottom). 

<img width="339" alt="Screen Shot 2022-04-18 at 2 42 32 PM" src="https://user-images.githubusercontent.com/99914793/163858074-e764a953-0b05-4f32-9594-e23c6420479e.png">

At the top, you can bind your hotkey to switch to this instance. I have mine set to Numpad 1. The first "Move and Click" action will maximise your instance. Press "Get" and wait for the countdown. Move your mouse to be on the top bar of the window.

![CURSOR](https://user-images.githubusercontent.com/99914793/163859733-599313f5-d293-4140-8d9d-73ef0fcabefb.jpg)

Wait for 5 seconds for Keyboard Maestro to capture your mouse coordinates. Next, go to the GUI Condition (Pause Until Conditions are Met). Double click the top of the window. It should maximize. Start resetting by pressing the gold boots, and pause. 

<img width="625" alt="Screen Shot 2022-04-18 at 3 01 48 PM" src="https://user-images.githubusercontent.com/99914793/163861020-077007fc-8b93-42c9-aa8f-92e73197bce5.png">

Press "Get" and put your mouse in the gray area of any gui button.

# Repeat these steps for each instance and corresponding macros.

Next, let's tackle the resetting macros. Open up "Reset all Instances". I have this bound to my "END" key, but you can change that. When you're on the wall, this will reset all instances. Set the first move and click to the "Quit World" button on the first instance (press get and wait). This should populate it with coordinates. The next move and click should be the same coordinates but off by one. Example:

<img width="638" alt="Screen Shot 2022-04-18 at 3 17 38 PM" src="https://user-images.githubusercontent.com/99914793/163863189-1cebc2ce-063e-4f18-9ba0-ee56563e6148.png">

There should be a pause, and then two move and click actions again. Do the same for these as the first two, but for the second instance. Repeat as needed.

<img width="640" alt="Screen Shot 2022-04-18 at 3 19 49 PM" src="https://user-images.githubusercontent.com/99914793/163863488-41934293-6a8a-4c71-b835-837d91771536.png">

At the end, set this to look like this (ONLY IF YOU HAVE MORE THAN ONE MONITOR).

Let's go to "Reset Instance 1". This is a bit more complicated. 

<img width="639" alt="Screen Shot 2022-04-18 at 3 20 59 PM" src="https://user-images.githubusercontent.com/99914793/163863653-1315b792-0eaa-4d6d-b447-978a05e87e96.png">

Maximize your first instance by double-clicking the top bar of the window. The pixel you need to get is the text that should say "Minecraft* 1.16.1". Click into the window, and get the text. Thanks to mac, that text will only be a certain color when the window is selected.

The "Return to Wall" action can have the same coordinates. Go down to the "Otherwise Execute the Following Actions". Minimize the instance window by double-clicking, and set this mouse movement like before (the first on the leave world button, the second one pixel off).

# Repeat for the rest of the reset macros.

## Wrapping Up

And you're done! You now should be able to run wall. To set up in the future, all you have to do is boot up your instances, use Spectacle to resize them, and add them as sources in Twitch Studio (just selecting the window in the screenshares).

If you have any questions, DM me on Discord (Blenor#0614).
