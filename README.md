<h1 align="center">Welcome to Forever in the Basement, a Minecraft server I (Johnams) am hosting on my personal homelab.</h1>

Forever in the Basement is a 24/7 "vanilla" Minecraft server that I would like to keep hosting for as long as possible. The mods I am installing do not affect the core gameplay; instead, they aim to make the vanilla experience prettier and more fun to play.

These steps will install a modded Fabric installation to your Minecraft Launcher. These mods are required for Voxy (far render distance mod) and Simple Voice Chat (proximity voice chat). I also included some sound overhaul mods and resource packs I think improve vanilla's experience. You can edit / disable any of these mods in the in-game mod menu.

_Note:_  You do not **need** to install any of these mods to play on the server. The only **real** functionality you will miss out on is Simple Voice Chat. With that said, I strongly recommend playing with these mods. If performance is a concern, simply disable shaders in-game.

This installs: (on 1.21.11)
<ul>
	<li>Mod Menu</li> 
	<li>Sodium, Iris</li> 
	<li>Voxy, Simple Voice Chat</li> 
	<li>Sound Physics Remastered, Prescence Footsteps, Ambient Sounds, WaveyCapes, LambdaBetterGrass, Shoulder Surfing</li>
	<li>EMF, ETF, Continuity, Proton Shaders, FallingLeaves</li>
	<li>FreshAnimations, Vanilla Mashup, Round Trees, Better Leaves</li>
	<li>Fabric API, Cloth Config API, ForgeConfig API, CreativeCore, EntityCulling, CullLeaves</li>	
	<li>Pre-generated world file required for Voxy</li>
</ul>

Server-Side Mods:
<ul>
	<li>Chunky, Simple Voice Chat, Lithium</li>
</ul>

<h2 align="center">World Explanation: Skip to Installation Steps if you don't care!</h2>


Voxy adds LODs to Minecraft. You can see extremely far with little impact to performance. The LODs are rendered client-side, meaning you cannot see other players or changes from other players until you visit them within the "real" render distance (10 chunks). I wish this was something I could improve, but for now Voxy is a client-side mod only.

On the server, I set a square world border & pre-generated all chunks 16,000 blocks wide (8,000 block radius from spawn). This means you cannot travel past X & Y: 8000 to -8000. This is for server performance, Voxy, and to allow future Minecraft content to generate outside of the border. I can edit this border later, but this is the starting point for practicality.

The Nether's world border is set to 8,000 blocks wide (4,000 radius). If you portal from the Nether outside of X & Y +/- 1000, you will end up at a world border.
The End has a world border of 8,000 blocks wide (4,000 radius).

The seed I chose for the Minecraft world should contain all current biomes within this range. With Voxy, you can just look for the biome from the sky!

Additionally: this adds Simple Voice Chat, which enables proximity voice chat in-game. The proximity chat is further enhanced with Sound Physics Remastered, which allows for echoes in caves and other fun effects.

<h2 align="center">Installation Steps</h2>

**<p align="center">DONT WORRY! YOU NEED TO DO VERY LITTLE TO GET THIS UP AND RUNNING SMOOTHLY (I DID IT FOR YOU!)</p>**

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

2. Download the "foreverinthebasement-main.zip" from the GitHub page. (Code > Download ZIP)
3. Download the world file from my Google Drive link (7.9gb): https://drive.google.com/file/d/1NtHjbWihnT8BWKbAXl0NzH4kYuLQpM5o/view?usp=sharing
4. The file is 7.9gb because the entire 16K world border is pre-generated.

5. Extract & move files to your .minecraft folder:

	1. Extract all contents of this zip file if you haven't already.
 	2. Extract the contents of "FITB Voxy World File.zip"
	3. Open C:\Users\\$YOURUSER\AppData\Roaming\\.minecraft (press Windows key, type %appdata%, click .minecraft)
	4. Make sure your ~\\.minecraft\mods folder is empty before copying anything over.
	5. Move all contents from this _foreverinthebasement-main\\.minecraft_ folder into your .minecraft directory.
 	6. Move all contents from the _FITB Voxy World File\\.minecraft_ into your .minecraft directory.


<h2 align="center">That's it for files!</h2>

4. Start Minecraft Launcher. Make sure "Fabric Loader 1.21.11" is selected on the bottom left, then click "Play"
5. Setup Simple Voice Chat in-game:

	1. Join the server.
	2. Press V to setup and edit Simple Voice Chat. 

6. Setup Voxy:
	1. In the server chat, type:
	2. 		/voxy import world "Forever in the Basement Voxy/"
	3. Wait for Voxy to import the LODs from the singleplayer world. This will take a few minutes, as it loads LODs for over 1 million chunks. Try not to open or close any programs during this time, as it can be resource-intensive until it finishes.
	4. That's it! Do not import the LODs again in the future, as this will overwrite the LODs of anything changed while you play. If a player builds across a mountain range, you will not see it in the LODs until you visit them.
    5. If you experience large cubes (LODs not rendering correctly), simply restart Minecraft.
 	6. Voxy's default "render" distance is 128 chunks. You can edit this in Options > Video Settings > Voxy > Rendering > Render distance. This is hardware 	   dependent. My sweet spot appears to be 1024 chunks. Yours may be higher or lower, the max is 2048 chunks!
 	7. Do not join or play the singleplayer world, as this may cause conflicts in the future.

8. Enable Resource Packs:
	
	1. Go to Options > Resource Packs
	2. Enable, in order:
		1. Vanilla Mashup
  		2. Round Trees (ignore compatability warning)
  		3. Better Leaves
  		4. Ubobtrusive Weather (ignore compatability warning)
  		5. Gentler Weather Sounds
		3. Fresh Animations
		4. FA All Extensions
  		5. FA Player
    3. When finished, the resource packs should appear in the list in reverse-order to above. These are just my preference, you can disable any packs or add your own, it does not matter (but the order of the packs does).

9. Enable Shaders: Use proton-voxy-support.zip

	1. In the pause menu, go to: Options > Video Settings > Shader Packs > photon-voxy-support.zip
	2. Select & click Apply.
 	3. Press K in-game to quickly enable or disable shaders.



If Voxy is not working in the End, type this command while in the End:
	**/voxy import raw "saves/Forever in the Basement Voxy/DIM1/region"**



<h3 align="center">THATS IT! Find a mountain, look around, and have fun!</h3>
<p align="center">Please report any issues, lag, or suggestions to Johnyams on Discord, or openly to #minecraft-chatroom</p>
<p align="center">Keep in mind this server is running off of my home internet. You will experience occasional lag spikes and high ping (when I'm downloading games!). You are connecting to a reverse-proxy VPS with WireGuard tunneling, not my home network. This server costs me less than $1/mo to host.</p>
