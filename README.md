# Final-Project
From Java Programming class MCTC


Final Project Game ReadMe

This program is a game in the style of a MUD (multi-user dungeon). It is a role-playing game set in a medieval fantasy environment. It is command line based with a graphical map that shows your location in the game world. The game is played by typing commands into the command line. You type 'north' to move north a room and 'west' to move west and so with the other cardinal directins. You will be given the name of the room you are currently in followed by a description of your surroundings. Objects you can interact with are listed after that. To interact with an object, you type an action followed by the name of the item. For example, 'take apple' or 'talk villager'.
Required setup:
The game makes use of a database to store the player info. The only thing you will need to run the game with the database is to create a mysql database named 'GameDB' and create a user with the name of 'Test' and a password of 'password' and give all grants to this user for the database GameDB. This should be the only required set up in order to use the game. Multiple players can be created and stored in this database so a person can have more than one character to play with. To start a new game, run Game.java.
It is recommended to move the command prompt window out of the way of the map GUI when it appears so you can type commands and see the GUI at the same time.
You will need to enter 'new' when prompted to create a new character and follow the prompts until you are put into the game world at which point the map GUI will appear.
 

Game mechanics:
There are three classes your character can choose from, they are standard RPG archetypes: warrior, rogue, and mage. Each has different strengths and weaknesses. 
Your character will have stats that govern your character.
HP or health, is the measure of how healthy your character is. When it reaches 0, you will die and the game will end. You receive damage to your HP (health points) from enemies or environmental hazards.
SP or stamina points, is your character's level of fatigue. certain actions need SP to be performed. For example, you may not be able to attack if your SP is too low. Any action requiring physical exertion will deplete your SP.
MP or magic points, is your pool of magical energy used to cast spells. note: this feature is not utilized in this game yet.
Strength- the measure of your character's overall might. The more strength you have, the more damage you can deal with melee weapons.
Dextarity- the measure of your character's deftness and hand-eye coordination. This determines certain action's outcomes such as how easy it is to land a hit on an opponent in combat.
Agility- how nimble and quick you are to move. Typically comes into lay in combat, how hard you are to hit.
Experience- how much experience your character has from combat and completing other tasks. Certain levels of experience allow you to increase in level allowing you increased stats and new skills and abilities.

Known Issues:
When restoring a saved character, even though x and y are saved in database, game always starts in startingRoom. 
Can't equip weapons, only armor
Room title text in GUI covers rooms


Future Features:
Save items in inventory to database
implement help system by typing 'help <search string for topic>' perhaps read in from text file
Maybe make single player version with saved info to encrypted text files so users can't edit their stats and cheat.
For multiplayer version, Put database on external server and have client apps connect to it.
Sound effects- sound effects for events in game, combat, ambient sound, etc. Even music, wav files stored in game directory.
Graphics- some pictures when enter rooms to show image of room.
Add command prompt entry into GUI- entering commands into GUI text field rather than having two separate windows for the game.
World map and local area map.
Add currency and shop keepers
Item modification- modify items attributes for example, sword does 5 damage, taking it to a smith and having it sharpened increases the damage of that sword object to 7, enchanting armor gives extra magical protection.
Weight based inventory- player can only carry so much inventory weight based on their strength.
Hunger system? Thirst system?
Definitely quest system
