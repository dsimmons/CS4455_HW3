## Team Tower Defense Reloaded

### Team Members:

- Brandon Whitehead <brandon.whitehead@gatech.edu>
- Dan Simmons <dsimmons@gatech.edu>
- Jeffrey Portman <jportman@gatech.edu>
- Alex Trevor <atrevor@gatech.edu>

### Requirements Met:

- *Two or more instances of the game should establish connections to each
  other.*
- *The initial game state should be synchronized.*
- *The game should communicate all changes in state as the game
  progresses.*


  **Known issue**: initial state and subsequent synchronization is in-place
  and working great.  One issue we're having that we were
  unable to fix prior to the submission was that the character object
  animations weren't being displayed between clients -- the movement
  was present (looks as if players are gliding), but not the respective specific animations. We should be
  able to figure out a solution before our next deliverable.

### Install Instructions:
  Nothing special.  The Web Player should be straightforward and building the Unity project should work as well.  Let us know if you have issues!

### Instructions To Grader:

**n** to bring up the networking prompt.  Have one copy of Unity run
"*Be Server*" and the other run "*Connect To Server*" to demonstrate network
capability.  For the sake of the Web Player or a single Unity instance,
"*Be Server*" essentially functions as a local-only game while no one is
connected.

***ASWD*** to move around.  ***Shift*** to sprint.  ***c*** to create one of
the three towers of various respective types. ***Fire2*** (usually right click) to use knock-back effect (use the cylinders in the game to demonstrate).  ***Right CTRL*** to use the player's ability to shoot projectiles.

**Objective:** Enemies spawn from the red particle effect across the
map.  Their behavior is to pathfind around the terrain and/or obstacles
(namely, towers) towards the lighter particle effect, the destination.
The objective of the game is to thwart their attempts at accomplishing
the latter by strategically placing towers of various rates of fire,
damage types, etc... across the terrain.

**Note:** Many game mechanics are proof-of-concept to some degree,
namely tower creation/placement.  Currently there are no time, space, or
resource limitations on placing new towers.  Further, towers presently
have a very far (almost inifinite) projectle range with placeholder
damage modifiers that simply shoot the closest enemy to them at any
point in time.  Enemies currently spawn in somewhat of fixed increments
of times rather than in "levels" or "waves" like we envision they will
eventually.

Currently, the focus was mainly on getting rudementary
pathfinding, networking, and physics incorporated into the game, along
with base game mechanics. Our plan going forth is to further refine the
aforementioned and hammer out the rest of the functionality before our
next/final deliverable.

### Scene To Open:
"Prototype" scene.

### Web Page URL:
http://dsimmons.github.com/CS4455_HW4
