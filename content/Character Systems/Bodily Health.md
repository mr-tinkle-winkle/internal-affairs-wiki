Every robot has 17 'parts'. Not to say there are 17 parts on the model (as each part may have more or less moving pieces).

Special affects for damage will be listed under each category, as well as the  'Effective/Ineffective Damage Types'. 
- Effective Damage Type will do more damage to that specific area, while non-effective damage types will do less damage. 
	- Specifically, non-effective damage types do 1x damage, while effective damage types do 3x damage.
	- Some may not have effective damage types.
	- An 'Ineffective' damage type means that it deals 1/3 of the damage.
		- Ineffective damage types have no chance of playing VFX.
The damage types, and what causes them, are as follows :
- Impact
	- Caused by sudden acceleration of the limb in any direction. This is the 'default' damage type.
		- To be clear, there is a check ran whenever a collision occurs. Without being extremely accurate, the code would look something like this:
			- OLD_VEL = 0
			- MIN_ACCEL_FOR_DMG = some fine tuned value
			- ACCEL_DMG_MUILT = some fine tuned value
			- When the player collides with an object,
				- If (CURRENT_VEL - OLD_VEL) > MIN_ACCEL_FOR_DMG
					- DMG = (CURRENT_VEL - OLD_VEL) * ACCEL_DMG_MULT
					- If DMG > (the limbs max hp)
						- If limb is fatal limb, kill player.
						- If limb is non fatal limb, do not kill player.
				- OLD_VEL = CURRENT_VEL
	- Plays any of the following onomatopoeia vfx, based on specifically what hit (each thing can play some of these)
		- WHAM!
		- SLAM!
		- BAM!
		- CRAAAK!
		- WHACK!
		- BANG!
- Sharp
	- Caused by something 'sharp' moving through or along the limb at a fast speed.
	- This damage type corresponds with bullets and anything else that is 'sharp'.
	- Plays any of the following onomatopoeia vfx, based specifically on what hit (each thing can play some of these)
		- SHINK!
		- SWISH!
		- SNIP!
		- RIIIIP!
The specific HP of each limb depends on the Robot being played as.


Symmetrical Parts (x2)
- Upper Arm
	- Impact Damage is ineffective.
- Forearm
	- Impact Damage is ineffective.
- Hand
	- Impact Damage is ineffective.
- Upper Leg
	- Impact Damage is ineffective.
- Lower Leg
	- Impact Damage is ineffective.
- Foot
	- Impact Damage is ineffective.
Non-Symmetrical Parts
- Head
	- Impact Damage is effective.
		- If you kill somebody via the Head with Impact Damage (but without enough 'overkill damage'), they will instead be knocked out.
	- The player dies immediately if this limb runs out of hp.
	- This limb will cause the player to be 'concussed' upon taking damage, which will reduce the players' strength and 
		- Concussions will cause the players' eyes to spin around.
- Neck
	- Sharp Damage is effective.
- Chest
- Lumbar
- Abdomen
	- Impact Damage is effective.