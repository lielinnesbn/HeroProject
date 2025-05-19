Project Title: Waypoint Camera & Enemy AI System
Developer: Liel Ben Noon
Course: CSS 385 – Interactive Media
WebGL Build: https://lielinnesbn.github.io/HeroProject/ 
Overview
This project builds on top of a previous interactive media assignment by introducing dynamic interactions between the Hero, Waypoints (Eggs), and Enemies. It focuses on advanced game mechanics like camera transitions, object state changes, and behavior trees for AI.
Controls
Arrow pad : Move the Hero character


Mouse Left Click: Shoot projectiles (to hit Eggs and Enemies)


Esc: Pause menu / Quit (if implemented)


Main Features Implemented
Waypoint Interactions (Eggs):


On collision with a projectile, the Egg object shakes at 10 cycles per second with increasing duration and magnitude:


1st hit: 1s, magnitude 1x1


2nd hit: 2s, magnitude 2x2


3rd hit: 3s, magnitude 3x3


Waypoint Camera:


Activates each time a Waypoint is hit.


Displays a label with the current status of the waypoint.


Enemy Behavior:


On Hero collision: Enemy rotates counter-clockwise → clockwise → enters Chase state (if Hero is within 40 units).


On Egg collision:


First hit – enemy stunned, rotates clockwise


Second hit – transforms into an Egg


Third hit – enemy respawns at origin or predefined spawn point


Development Time
The project was completed over the course of 4 days. Development was divided as follows:
Day 1: Setup and initial integration of previous project elements


Day 2: Waypoint shaking and camera transitions


Day 3: Enemy behavior scripting and testing


Day 4: Debugging, polishing, and WebGL deployment


Challenges and What I Learned
One of the most challenging parts of this project was correctly handling multiple states and transitions for the enemies. Ensuring each collision led to the right response (especially chaining the enemy stun → egg → respawn logic) required careful use of Unity's state management and coroutine features.
Another tricky component was implementing the camera transitions that would not interrupt gameplay but still provide a clear visual feedback for Waypoint interactions. I learned to better use camera priority layers, Cinemachine components, and label UI to support player awareness.
Reflection:
 This assignment taught me the importance of state machines in game development and how to enhance player feedback using animations and visual cues. It also helped me deepen my understanding of collision handling, coroutines, and camera systems in Unity.
