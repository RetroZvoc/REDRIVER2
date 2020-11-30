# REDRIVER2 (RetroZvoc's fork)

This is a fork of SoapyMan's REDRIVER2.
This fork is made as a mod of REDRIVER2 dedicated to RetroZvoc's mods.

### Mods to implement
- Perfect invincibility (no drowning, no Black Screen of Death, unflip instead of getting wrecked, be able to get out of a flipped car, and never take too much damage)
- Unlimited upward velocity (skip web effect)
- Unlimited angular velocity
- Explosive cop cars when wrecked
- 2-player freeroam
- 2-player co-op undercover
- 2-player on-foot action
- Everything unlocked (towns, missions, cars, cheats, race tracks, debug menu, doors, gates, garages, switches, everything!)
- 2-player gamemodes (assisted or versus of quick chase, quick getaway, survival, etc.)
- Shift Existance (similar to Driver San Francisco; possibly with a floaty camera vision)
- Better Film Director for multiplayer (in multiplayer pause/gameover menu, no camera boundary/distance restrictions, better control, show/hide HUD, change Sfx/Music volume)
- and more...

### Original notice

PC (Windows):
[![Build status](https://ci.appveyor.com/api/projects/status/9abepvls6jexapqy/branch/master?svg=true)](https://ci.appveyor.com/project/SoapyMan/redriver2-10jm8/branch/master)
<p align="center">
<a href="https://streamable.com/rtjpoa"><img src="https://i.ibb.co/MG8qwqx/aaa.png"/><a>
 </p>

 PSX: pending
 
Project attempting to reverse-engineer PS1 game Driver 2;

Start Date: 28 March 2019

### Goals
- Rebuild all source code from assembly
- Compile native version for **PC** (and for **PSX** later)
- Make game playable from start to finish, all game modes should function properly
- Fix all reverse-engineering **bugs**
- Fix some existing critical bugs and performance issues
- ***OpenDriver2?*** rewrite code, implement various cool stuff, PC rendering and audio engine, get rid of hard-coded stuff

### How is it done?
- All information (variables, types and function names) have been obtained from debugging symbols (.SYM), driver_psx_level and DLE
- Ghidra project (based on Italian SYM) to deal with overlays, simple code complex branching - semi-auto decompilation
- IDB based on Spanish SYM when dealing with things Ghidra can't handle properly - manual decompilation (mostly GTE code)
- Originally targeted *Playstation* game built upon [Psy-X (Psy-Cross) (formely extended TOMB5 emulator)](https://github.com/OpenDriver2/REDRIVER2/tree/master/src_rebuild/PsyX)

### How to use
See [Wiki/Installation Instructions](https://github.com/OpenDriver2/REDRIVER2/wiki/Installation-instructions)


### Credits
- RetroZvoc - mod programmer for this fork
- Soapy - lead programmer (of the original REDRIVER2)
- Fireboyd78 - code refactoring and improvements
- Krishty, someone972 - formats decoding
- Gh0stBlade - API-level PSY-Q libraries reimplementation (HLE PSX Emulator) [(link)](https://github.com/tomb5/tomb5)
- Ben Lincoln - [This Dust Remembers What It Once Was](https://www.beneaththewaves.net/Software/This_Dust_Remembers_What_It_Once_Was.html) (*TDR*)
- Stohrendorf - [Symdump](https://github.com/stohrendorf/symdump) utility