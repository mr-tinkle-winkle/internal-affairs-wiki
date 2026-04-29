# Base Movement Inputs
- WASD = Walking in any direction (kinda obvious)
- SPACE = Jump
	- The player can hold space for a more powerful jump. The players' hands will raise while preparing a jump.
	- Jumping just kicks the players feet down with force. If there is nothing below the player, the jump will look to the sides for walls to kick off of. If it finds a wall, it will kick off forward and upwards, with a slight outward push obviously.
- Z = Ragdoll (hold by default, toggle option in settings)
- CTRL = Crouch
	- Crouch also makes the player attempt to stand up.
- Scroll = 'Change Movement Mode'
	- Aim/Focus
		- This will cause the player to aim any weapon held. If they are holding a melee weapon, it will hold it in a threatening pose.
		- If the player is not holding a weapon, but they are holding a prop, the prop will be lowered and the player will focus.
		- If the player is holding nothing, the player will focus.
		- Regardless of which focus activates, the players' eyes will zoom when focusing.
	- Walk
		- This will make the player stand up straight.
		- In this mode, the players' walk speed is lowered.
	- Run
		- The player will lower their center of gravity.
		- In this mode, the players' speed is significantly increased.

# Movement Design
The players' limbs can only move via rotation. They are put together with rotors and springs.
Our characters will generally have less felt inertia than Sub Rosa characters.