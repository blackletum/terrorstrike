## !!!
If you experience issues with the game rendering your hud gun sprites/hud whatevers with everything being the CS Title font, check your installed Fonts (if you're on Windows) since CS:S uses fonts to render things, it prioritizes the fonts you have installed on your machine over the ones in the sourcemod's \resource\ folder (for some reason.)

## New Readme:
This repo fixes bot pathfinding and ragdoll crashes. It also reimplements valves prototype gamemode for left 4 dead. Terror-Strike or Terror.
You must add the TERROR macro to the server project to enable this.

## My game crashes!
First make sure you have Counter-Strike: Source installed.
If this is while loading a map it might be an unsupported navmesh file version. Remove this file and try again.

## nrk's summary of the original CS:S community readme

**Counter Strike Source: Community Edition** is open source port of the leaked 2007 Source engine leak of CS:Source.
This mod was originally made to transition everybody from CS:S to CS:S:CE, but you can see how well *that* worked out.

### Goals

- [x] Finish the port of the game to Source 2013
- [ ] Make fully functional the cut VIP mode so everyone can play it without server plugins
- [ ] Make fully functional the cut Prison Scape so everyone can play it without server plugins
- [ ] Implement a DM mode like CSPromod
- [ ] Redo the Bots and hostage’s AI using the [(Nextbot System)](https://developer.valvesoftware.com/wiki/NextBot)
- [ ] Implement the Vote System so everyone can vote without using plugins
- [ ] Implement Class Based Hands Like CSGO
- [ ] Implement CSPromod's Shadows RTT
- [ ] Bring back to life the shield. [According to Billy; adding the molotov SUCKED, so re-implementing the shield is gonna suck even harder.]

### Bug

- The prop’s physics is a little... estranged... well sometimes you pass the entire prop but other times the prop push the player.
- The round DONT end don't import if the time is 0:00 just the round doesn’t end.
- The flashbang doesn’t disappear sometimes.
- The Animation system used in the leak is the same in the HL2MP it used the base_playeranimstate so this animsystem don’t come whit a MP support so you can see the player making the walk anim but stuck at the first frame.
  The only way to fix this is redo the animation system to make work whit multiplayer_animstates.
- The lighting in the classmenu for the models is bugged don’t used the color white it used estranged colors.
- The Dynamic crosshair it’s not the same to the he original CSS someone of the cvars don’t work.
- Using the Bots may cause the game crash. 

### --- these bits are from NRKCEG2!! ---

### nrk's to do list:
 - [x] add T-side weapons to CT buy menu for balancing
 - [x] try and figure out why my local copy has a weird font loading bug
 - [ ] update some more UI elements
 - [ ] ask billy if I can start contributing to the mod proper instead of just messing around on my fork
 - [ ] figure out how pull requests work then send one over
 - [x] make more terror-strike purists mad by making more UI and balance changes (even if they're for the better)
 - [ ] upload my config for those who want to fiddle with Hammer.

### Things I need to figure out:

- [ ] Why is Medium.OTF (a CS:GO font) in the resource folder, and when is it used?
- [ ] How to code in C++ since practically all of the game's code is written in it, so for me to make any major modification I'd need to learn Source SDK and C++.
- [ ] Figure out if Medium.OTF is even used by the game at all, since it doesn't seem like OpenType (OTF) is recognized by CS:S since it's fonts use TrueType (TTF)

### hehehehehehe
<img src="https://github.com/nrkceg2/terrorstrike/blob/main/~misc-whatevers/funny-number.png?raw=true">
(as of 03 December 2024 @ 11:06:06 AM UTC-5 [Eastern Standard Time])

### Credits

|           **Valve**            |           Source Engine and Counter Strike Source            |
| :----------------------------: | :----------------------------------------------------------: |
| **Joshua Ashton And SCell555** |            **Original creator of SourcePlusPlus**            |
|         **PeterScout**         | **Modified SourcePlusPlus's CSS (witch is based this port)** |
|         **NicolasDe**          |                 **For his amazing GameUI2**                  |
|        **TotallyMehis**        | **Creator of Zombie Master: Reborn and some code that is used here** |
|         **Spirrwell**          |                   **FMOD Implementation**                    |
|         **BillySB**          |                   **Basic Terror-Strike gamemode** ...<sub>and generally being a cool guy.</sub>                    |
|         **Sregor**          |                   **Left 4 Dead common infected player models.**                    |
|   **FriskTheFallenHuman**   |                **Original cscommunity repo that this fork builds on**    |
|         **nrkceg2**         |     **motd, gameinfo, ~~eating~~ modding a lot of res files, and weapon stuffs.**       |
