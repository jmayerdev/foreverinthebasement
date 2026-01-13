<h1 align="center">Welcome to Forever in the Basement, a Minecraft server I (Johnyams) am hosting on my personal homelab.</h1>

Forever in the Basement is a 24/7 "vanilla" Minecraft server that I would like to keep hosting for years to come. The mods I am installing do not affect the core gameplay; instead, they aim to make the vanilla experience prettier and just more fun to play.

These steps will install a modded Fabric installation to your Minecraft Launcher. These mods are required for Voxy (far render distance mod) and Simple Voice Chat (proximity voice chat). I also included some sound overhaul mods and resource packs I think improve vanilla's experience. You can edit / disable any of these mods in the in-game mod menu.

_Note:_  You do not **need** to install any of these mods to play on the server. The only **real** functionality you will miss out on is Simple Voice Chat. With that said, I strongly recommend playing with these mods. If performance is a concern, simply disable shaders in-game.

This installs: (on 1.21.11)
<ul>
<li>Fabric API, Cloth Config API, Mod Menu,</li> 
<li>Sodium, Iris,</li> 
<li>Voxy, Simple Voice Chat,</li> 
<li>Sound Physics Remastered, Prescence Footsteps, Ambient Sounds, CreativeCore,</li>
<li>EMF, ETF, Continuity, FreshAnimations, Ultimacraft, Complementary Unbound, Proton</li>

<li>as well as a pre-generated world file required for Voxy.</li>
</ul>

<h2 align="center">World Explanation: Skip to Installation Steps if you don't care!</h2>


Voxy adds LODs to Minecraft. You can see extremely far. The LODs are rendered client-side, meaning you cannot see other players or changes from other players until you visit them within the "real" render distance (10 chunks). I wish this was something I could improve, but for now Voxy is a client-side mod only.

On the server, I set a square world border & pre-generated all chunks 16,000 blocks wide (8,000 block radius from spawn). This means you cannot travel past X & Y: 8000 to -8000. This is for server performance, Voxy, and to allow future Minecraft content to generate outside of the border. I can edit this border later, but this is the starting point for practicality.

The Nether's world border is set to 10,000 blocks wide (5,000 radius). If you portal from the Nether outside of X & Y +/- 1000, you will end up at a world border.
The End has a world border of 10,000 blocks wide (5,000 radius).

The seed I chose for the Minecraft world should contain all current biomes within this range. With Voxy, you can just look for the biome from the sky!

Additionally: this adds Simple Voice Chat, which enables proximity voice chat in-game. The proximity chat is further enhanced with Sound Physics Remastered, which allows for echoes in caves and other fun effects.

<h2 align="center">Installation Steps</h2>

**<p align="center">DONT WORRY! YOU NEED TO DO VERY LITTLE TO GET THIS UP AND RUNNING SMOOTHLY (I DID IT FOR YOU!)
ESTIMATED: 5 MINUTES</p>**

<p align="center">If you know what you're doing, you can install these mods with whatever launcher you prefer. You will still need the pre-generated world file for Voxy to work. Otherwise:</p>

1. Install Fabric:

	1. Download / update your Minecraft Launcher.
	2. Once downloaded / updated, close the Minecraft Launcher.
	3. Download the Fabric installer from:  https://fabricmc.net/use/installer/
	4. Download for Windows & run Installer. In the installer:
	5. Make sure "Client" is selected (default).
	6. Minecraft Version: 1.21.11
	7. Loader Version: 0.18.4
	8. Launcher Location: C:\Users\\$YOURUSER\AppData\Roaming\\.minecraft (default).
	9. Make sure "Create Profile" is checked.
	10. Make sure Minecraft Launcher is not open in the background.
	11. Click "Install"

2. Download the "Forever-in-the-Basement-Config.zip" from the GitHub page. The file is large due to the pre-generated world file.

3. Extract & move files to your .minecraft folder:

	1. Extract all contents of this zip file if you haven't already.
	2. Open C:\Users\\$YOURUSER\AppData\Roaming\\.minecraft
	3. Make sure your ~\\.minecraft\mods folder is empty before copying anything over.
	4. Copy all contents from this .minecraft folder into your .minecraft directory.


<h2 align="center">That's it for files!</h2>


4. Setup Simple Voice Chat in-game:

	1. Join the server.
	2. Press V to setup and edit Simple Voice Chat. 

5. Setup Voxy:

	1. In the server chat, type: /voxy import world "Forever in the Basement Voxy/"
		(when the options appear, use your arrow keys to select the world, then press tab to confirm)
	2. Wait for Voxy to import the LODs from the singleplayer world. This will take a few minutes.
	3. That's it! Do not import the LODs again in the future, as this will overwrite the LODs of anything changed while you play. If a player builds across a mountain range, you will not see it in the LODs until you visit them. 

6. Enable Resource Packs:
	
	1. Go to Options > Resource Packs
	2. Enable, in order:
		1. Ultimacraft
		2. Fresh Animations
		3. FA All Extensions
	   Ultimacraft should be on the bottom of the list, followed by Fresh Animations, then FA All Extensions.

7. Enable Shaders: Use proton-voxy-support.zip

	1. In the pause menu, go to: Options > Video Settings > Shader Packs > photon-voxy-support.zip
	2. Select & click Apply.
	3. I also included a modified version of the Complementary Unbound shader pack. This shader is not officially supported for Voxy, but I like it. Feel free to try it out, but it may cause some visual bugs with distant terrain.

<h3 align="center">THATS IT! Find a mountain, look around, and have fun!</h3>
<p align="center">Please report any issues, lag, or suggestions to Johnyams on Discord, or openly to #minecraft-chatroom</p>
