# Goodvibes.Assets.Pishock
Reactive PiShock model and Remote for increased immersion in VR

## Contents
This package contains everything you need in order to setup PiShock for your very own VRC avatar. With everything found within this file you will be able to remote control yours or someone elses PiShock with the use of GoodVibes and get the immersion while doing it.

### This package contains:
- A rigged PiShock Model
- Textures
- Normals
- Emissionmaps
- Unity package

## Relies on
- VRCSDK 3.0
- Poiyomi Pro shader

## How it works
PiShock is a remote shocker for adult use and it's possible to control yours or someone elses PiShock using an API. GoodVibes have this already implemented in an easy to use interface (If you want to see how GoodVibes work please watch https://youtu.be/soi9iFwE3Bg). 
PiShock works in a way where you need to set the intensity and the duration of an action, you can have your master do this if you trust them completely or with the use of this prefab you can have your master control the action of your PiShock using Avatar Dynamics, while you're still in complete control of duration and intensity yourself. This package also contains everything you need as a master to remote control your pet/sub using the radial menu.

## How to set it up
The README.txt contains all information on how to set up the PiShock and the Remote if you happen to lose this repository.

### Setup the Shocker
1. Drag the PiShock prefab into the root of your avatar
2. Unpack the prefab completely
3. Scale and place the PiShock by the Neck, or wherever you want it
4. Drag the neck bone(or whatever bone is closer) into the Parent Constraint component on the PiShock object
5. Click "Is Active" and "Lock" on the Parent Constraint component
6. See steps below for how to merge the Controllers and setup the Parameters

### Setup the Remote
1. Drag the PiShock_Senders prefab into the root of your avatar
2. See steps below for how to merge the Controllers and setup the Parameters

### Merge controllers and setup parameters
1. Download and install VRLabs Avatars 3.0 Manager from https://github.com/VRLabs/Avatars-3.0-Manager
2. Navigate to _/GoodVibes/PiShock/Controllers_ in your project files
3. Go to one of the following directories depending if you set up the PiShock, the Remote or both
	- PiShockAndRemote
	- OnlyPiShock
	- OnlyRemote
4. Merge the controllers located in step 3 using VRLabs Avatars 3.0 Manager tool
5. Navigate to _/GoodVibes/PiShock/ExpressionParameters_ in your project files
6. Go to one of the following directories depending if you set up the PiShock, the Remote or both
	- PiShockAndRemote
	- OnlyPiShock
	- OnlyRemote
7. Add the parameters from the located parameter object into the parameters of your own avatar

### Setup the Expression Menu
1. Navigate to your avatars expression menu
2. Click "Add Control"
3. Name the new control "GoodVibes"
4. Add the "GoodVibesLogo_small" as the Icon
5. Make the type "Sub Menu"
6. Add "Menu GoodVibes" as the Sub Menu

### Notes
* The controllers are currently setup using "Write Defaults", it works just as well without it. If you're 
running into issues with your controller just disable "Write Defaults" on all the PiShock Controller Layers.

## Credits
- Zobbit (https://twitter.com/ZobbitPlots) for the PiShock base shape
- Yuwukii (https://twitter.com/YukiLewdie) for testing these instructions