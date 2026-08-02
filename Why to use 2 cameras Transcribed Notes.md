Transcribed Using Gemini

### Benefits of using Multiple Cameras



* **Perfect hit detection:** Adding side camera, solves the Z axis problem. Instead of guessing from a flat Id image, the system knows the exact millisecond the saber interacts with the block.


* **No Blockage:** Multiple angles eliminate blind spots. If a player crosses arms or blocks the front camera with their body, the side camera maintains the line of sight.


* **Dynamic Scoring:** Real time coordinates allow the system to calculate the exact velocity, trajectory, and angle of the swing. The game can reward players for force or accuracy of their swings.


* **Full-Body Dodging:** Multiple feeds allow the AI to generate a rough 3D bounding box of the player. This can allow dodging mechanics.



---

### Why not 1 camera?



A single camera can't accurately measure 3d depth (z-axis) which ruins the precise hit timing needed for a rhythm game. It also creates massive blind spots.

### Why not 3 cameras?



Because there are IMU sensors in the sabers, they can maintain perfect tracking of the swings and solve blind spots on their own. Adding a third camera would waste processing power and complicate the setup.
