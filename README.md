# Scenes
Scenes is a basic cutscene editor in minecraft. This script allows you to create great looking cutscenes with little effort. You can easily integrate them into other skripts.
## Dependencies
* skript-logs
* Skript (The Latest Version is Recomended!)
## How to Download
Before installing, make sure you have the required addons!
* Step 1: Download the 'scene.sk' file.
* Step 2: Upload it to plugins/Skript/scripts.
* Step 3: Type /sk reload scene
* Step 4: Complete!
## Documentation
#### Syntax
You can use this code to add scenes in your own scripts.
```
if {logLoc::%player%} is not set:
    startScene("Scene Name", player)
```
#### Example
This is an example using the syntax above. This shows you you can add on to the code.
```
on region enter:
    if "%region%" contains "Region Name":
        if {logLoc::%player%} is not set:
            startScene("test", player)
            play sound "ui.toast.challenge_complete" with volume .7 with pitch 1 at player's location for player
            send title "&b&lDiscovery!" with subtitle "&7You discovered a location!" to player for 7 seconds with fadein 1 second and fade out 1 second
```
