# **CS463 Virtual Reality Project - Old School RuneScape **

Demo Video: 
Task: Create an immersive VR experience that had interactables, and unique elements that showcases your creativity.

**Note**:
- I made this as a school project, used for non-commercial purposes. No copyright infringement was intended. If certain elements are buggy, I apologise, please be diplomatic about it. 
- This project has reached the end of development, so no more changes from me will be pushed out. Feel free to clone this repository and change it however you like, just remember to give credit where it's due.
- This project works with Unity 2022.3.211f and has not been tested with other versions of Unity. You can directly run the project on your PC
- I have managed to get this project running on a Meta Quest 3 after using USB debugging to get the ISO onto my Oculus Device. If you need more information, feel free to reach out.

## How it works
- All progrmamable behaviour of the Non-Playable Characters (NPCs) and what they dropped were mostly accomplished with C# programming and extensive online research in my own time, outside of class.
- NPC roaming behaviour was accomplished with a C# script and the NavMesh component, where the C# script allowed the NPCs to switch animation states when moving, giving the impression of walking and autonomy.
- Background music and SFX management fell under one C# script, which fed the Audio Listener certain sounds when certain criteria were met (NPC health reached 0, entering new region, etc).
- All environment and character assests were exported from the Old School RuneScape game cache under Fair Use, and all the interactions with the ground and other objects were configured by me.

## Features
- Free-roaming NPCs and 3D Interactable and Immersive environment.
  - Chop logs with an axe, burn them at a furnace, use keys, which are dropped by monsters, to unlock new areas.
  - Like in RuneScape, background music will change when players move to different areas. There are also proximity sounds, as demonstrated by the castle fountains.
  - Grey Teleportation portals disks around the game on the ground for ease of transport around the map.
- Simple combat system
  - 3 types of weapons (Steel dagger, Rune Scimitar, Osmumten's fang) which deal ascending amounts of damage in that order, which allows players to kill monsters quicker.
  - Some monsters, when defeated, will drop these weapons. Certain monsters can also drop useful items.
  - Fightable NPCs include: goblins, hill giants, and Elvarg, the dragon.


## Setup
*** There seems to be an issue with item grabbing, so currently the repo is not functional. I'll remove this message when it is resolved. Sorry about that :(
### Method 1: Running locally on your PC
1. Have Unity Hub and Unity **_2022.3.211f_** installed.
2. Clone the repo to your Unity working directory.
3. Under the "Viewers" GameObject, ensure that "XR Device Simulator" and "XR Origin (XR Rig)" are checked and visible. *Everything else should be greyed out.*
4. Under your "Game" tab, ensure that you are on "Display 8". This will be your main VR camera.
5. Click the "play" button to start. To move around, hold the "Shift" key and use WASD to move around. To grab an item, while holding "Shift", point the left controller to the item that you want to grab and hold the "G" key to grab it. Release the "G" key to drop it.

### Method 2: Build it and directly run it on your Meta Quest 3
1. Clone the repo and open the project in Unity.
2. Under the "Viewers" GameObject, ensure that "XR Device Simulator" and "XR Origin (XR Rig)" are checked and visible.
3. Connect your Meta Quest to your PC and ensure that USB debugging is switched on (see online on a guide on how to turn it on).
4. In Unity, go under "File > Build Settings".
5. Select "Android" as your platform and under "Run Device", select your Oculus Device.
6. Click "Build and Run". After building, the project should be loaded onto the Meta Quest 3.
