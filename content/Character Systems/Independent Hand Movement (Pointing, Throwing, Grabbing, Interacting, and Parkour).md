When the player holds Q, their left hand will extend. When they hold E, their right hand will extend. With their hand extended, moving their mouse will move where their hand is. If the hand moves too far outside of the players vision, the player will turn (via Free-Look) to look in the direction of the hands. The players' torso will turn before their head in Free-Look, but that will also only happen if it extends past a certain point.

With that established, here is how the system applies to each function.
# Pointing
- The player can point by doing this with an empty hand. Not much to say here. Nothing special even needs to be added for this.
- On the topic of free hand movement, it is worth mentioning that if you have both hands extended AND one of them is holding onto something, the free hand will point while the 'used' hand will not move.
- The player can control the distance they hold out their hand at by scrolling while holding alt.
# Throwing
- By moving the hand and letting go at the same time, the player can throw whatever is in their hand. Nothing special needs to be added for this either.
	- The player can let go by ALT + Clicking the hand that they want to drop an item in. This will not interact with the item (e.g. dropping a gun will not shoot the gun).
# Grabbing
- If the player holds Click, the corresponding hand will Grab. Grabbing works on literally anything by default, although it can be disabled in order to not work with specific things.
	- Grabbing the world only works if grabbing an edge.
		- 'Edge' detection, if not automatically supported by the game, will just be 'if any of the connected faces have a >60 degree deviation from this face'.
# Interacting
- If the player grabs an interactable object, it will automatically be interacted with. 
- If the player grabs an item that can be picked up, the player will automatically pick it up and it will go into one of their inventory slots.
# Parkour
- Holding Jump while grabbing and object will cause you to pull up. This can be used to climb walls, swing to prepare for poles, or whatever. The player will pull up in the direction of their movement, or just straight up if they are not moving in any direction.
- If the player holds crouch while doing a Pull Up, they will instead only bend their arms.
- The 'purpose' of this is to allow the player more fine control of their limbs, allowing things like monkey bars.
- Holding a movement key while held onto an object and airborne will cause the player to swing slightly in the direction that they hold. The player can do these back and forth to actually get some good momentum.