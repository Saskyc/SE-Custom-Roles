# SE-Custom-Roles
Custom Roles script that can be used to create new roles


## Explanation of code for dummies:

* `STOPIF {CHANCE100} <= 10` // This has 10% to stop the script if you make it 20 than 20% so the default role has 90% of spawning
  
* `STOPIF {SCIENTIST} >= 1` // So this basically sees if there is enough scientists so it basically chekcs if there is any if you would want to have minimally 4 than just set it to 4
  
* `PLAYERVAR SAVE {CUSTOMROLE_PLAYER} {RANDOM:SCIENTIST:1}` //This will save the Player Variable we want to use. I use scientist you can use whoever other you want just go here if you want: [SEPlayerVariables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Variables#player-variables)
  
* `SETROLE {CUSTOMROLE_PLAYER} ClassD 1` // So not if you want you can give them other [RoleTypes]([https://github.com/Thundermaker300/ScriptedEvents/wiki/Variables#player-variables](https://exiled-team.github.io/Web/docs/Resources/Intro#roletype-team-side-and-faction)https://exiled-team.github.io/Web/docs/Resources/Intro#roletype-team-side-and-faction) you want.
  
* `TPROOM {CUSTOMROLE_PLAYER} LczCafeteria` // So here you teleport them where you want I teleport the ClassD to PC15. If you want to change the LctCafeteria to something other you can go here: [RoomTypes](https://exiled-team.github.io/Web/docs/Resources/Intro#roomtype).
  
* `GIVE {CUSTOMROLE_PLAYER} GunCOM15 1` // So here is 4 lines I will describe only 1 but you can do more below it. If you want to change GunCOM15 again go here: [ItemTypes](https://exiled-team.github.io/Web/docs/Resources/Intro#itemtype). Than there is 1 that is the amound of ItemTypes you want to give player.
  
* `BROADCASTPLAYER {CUSTOMROLE_PLAYER}` 10 You are a custom role bla bla bla. // This is what you broadcast to player, also you can set the duration to other number than 10 (in seconds). [RichText](https://docs.unity3d.com/Packages/com.unity.textmeshpro@4.0/manual/RichText.html) can be used.
  
* `PLAYERVAR DELETE {CUSTOMROLE_PLAYER}` // Here you just delete the player from the role so other scripts can use it.

# License:
* 1-clause BSD License
* [I dont know how licenses work](https://opensource.org/license/bsd-1-clause/)
