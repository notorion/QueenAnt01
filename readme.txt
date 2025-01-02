Implemented new Queen Ant GrandBoss fight mechanics.

Hi!
This is the Queen Ant mechanics, based on live checks on the official server, Chronos.
[s]Return of The Queen Ant - Monday - Tuesday is in 9pm.
Hero’s Tome time respawn 10/2022 Queen Ant Monday 9pm[/s]

The script is only configured for the time of day Shinemaker: Respawn at 8pm on Mondays.

The battle:
Queen Ant is protected by a barrier, to destroy it requires 2000 attacks in 10 minutes. The barrier can return during the battle.
https://github.com/notorion/QueenAnt01/blob/main/%7B6ED9DA26-698C-4F52-9C4A-4167EADCCB8C%7D.png?raw=true
Queen Ant has two powerful initial attacks, I could see top players fall easily.

Queen Rage is a long-range targeted attack.

Ground Shaker is an area-of-effect attack that deals stun + damage.

At some point, when the Queen Ant has a certain HP, she will become furious, but unfortunately she will not call the worker ants. She will dig her claws into the ground and summon 'eruptions' on the ground. It is time for the player to move far away, because several tornadoes will emerge from there around the Queen Ant, causing significant damage.
https://github.com/notorion/QueenAnt01/blob/main/%7B7CA84ED8-8991-405B-BC89-AEB7350CD518%7D.png?raw=true

There is no way for the player to stand still.

Points to note and that may be modified throughout the L2 update;
In the current script:
On first contact with the Queen Ant;
Player below level 110 is teleported to Gludio.
Player outside the Command Channel is also teleported to Gludio.
When Queen Ant leaves or is taken out of the 'Lair', her HP resets and she is teleported to the respawn.
If any player manages to attack the Queen Ant in any way outside the 'Lair', he will be teleported to Gludio. (Custom).
The attack against Queen Ant can only be done in CC of at least 14 players.
Loot is not configured in this script.
Some new item debuffs and some skills are activated against the boss 100% by some trigger and can cause a 'Bug' during the battle. To get around this without changing the original 'improved immunity', I created the custom 'improved immunity' with id '9905099'. Common debuffs will work normally. Visually nothing changes, only the protection.


IMPORTANT!
In order for the script to work normally, spawning the boss without errors, it may be necessary to modify the existing DB.

Modify the following:
Table grandboss_data
respawn_time leave the value 0.
and save.
https://github.com/notorion/QueenAnt01/blob/main/db%20grandboss_data.jpg?raw=true
The script was written together with the grandboss table.

Before making it live, I test it to see how it behaves on your server.
On the Mobius base, it worked normally for a few weeks of testing.

Implemented new Queen Ant GrandBoss fighting mechanics

Hi!
This is the Queen Ant mechanics, based on live checks on the official server, Chronos.
Shinemaker:
Respawn at 9pm on Mondays.

Points to note and that may be modified throughout the L2 update;
In the current script:
On first contact with the Queen Ant;
Player below level 110 is teleported to Gludio.
Player outside the Command Channel is also teleported to Gludio.
When Queen Ant leaves or is taken out of the 'Lair', her HP resets and she is teleported to the respawn.
If any player manages to attack the Queen Ant in any way outside the 'Lair', he will be teleported to Gludio. (Custom).
The attack against Queen Ant can only be done in CC of at least 14 players.
Loot is not configured in this script.
Some new item debuffs and some skills are activated against the boss 100% by some trigger and can cause a 'Bug' during the battle. To get around this without changing the original 'improved immunity', I created the custom 'improved immunity' with id '9905099'. Common debuffs will work normally. Visually nothing changes, only the protection.

The battle:
Queen Ant is protected by a barrier, to destroy it requires 2000 attacks in 10 minutes. The barrier can return during the battle.

Queen Ant has two powerful initial attacks, I could see top players fall easily.

Queen Rage is a long-range targeted attack.

Ground Shaker is an area-of-effect attack that deals stun + damage.

At some point, when the Queen Ant has a certain HP, she will get furious, but unfortunately she will not call the worker ants. She will dig her claws into the ground and summon 'eruptions' on the ground. It is time for the player to move far away, because several tornadoes will emerge from there around the Queen Ant, causing significant damage.

The player cannot stand still.

IMPORTANT!
In order for the script to work normally, spawning the boss without errors, it may be necessary to modify the existing DB.
Modify the following:
Table grandboss_data
respawn_time leave the value 0.
and save.
The script was written together with the grandboss table.
Before making it live, I test it to see how it behaves on your server.
On the Mobius base, it worked normally for a few weeks of testing.

Have fun with your friends
