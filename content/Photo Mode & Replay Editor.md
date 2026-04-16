# Photo Mode
The player can enter Photo Mode through the menu. They can also set a keybind for it, but it is unbound by default.

Functions how you would expect. 
# Replay Editor
The player can enter a Skate 3 esque replay editor, also through the menu, also unbound by default but has a keybind.

- The host of the server has the option to allow or disallow server-side replay buffer.
	- This will choose if other players even have the option in the first place to offload the physics work to the host.
	- If the host allows it, it will follow the players' settings preference.
	- The setting is defaulted to client side replay buffer in order to spread out the load, but can be manually changed to server side for players on weak devices.
- By default, 'Replays' are 1 minute long.
	- The player can change this in settings, and the server can also set a limit to server-side replay buffer length.
- Replays save the entire worlds' physics state, and allows the player to view anywhere in the world.
- There is a rudimentary replay editor with support for:
	- Camera Keyframes
	- Scrubbing through the timeline
	- Changing beginning and ending
	- Exporting as text (exports physics states from beginning to end in a .txt)
	- Importing (imports above .txt files)
	- Exporting as video (defaults to mp4)