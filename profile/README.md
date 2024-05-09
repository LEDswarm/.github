![breadboard prototype illustration](https://ghoust.s3.fr-par.scw.cloud/swarm_prototype_banner4.png)

# A simple, but very engaging social game for groups

__*Tap mine, I'll tap yours!*__

LEDswarm is an interactive light-based game for groups, with controllers that react to movement, orientation and proximity.

For example, each person may hold a controller with a green light, which turns red if it is moved too quickly. The goal is to keep your own light green while pushing (softly) on the other light rods to make them red. Being green or red determines if you're still in the round or not.

The concept is based [overflo](https://github.com/overflo23)'s [`ghoust`](https://github.com/Ghoust-game/ghoust) game, and especially the Last One Standing game mode is derived from the original version.

# Game Modes

* ### Territory

All players are divided into two or more groups and each group is assigned a color. To take over territory, get close to another controller within a configured range, try to tap it and it will take on the color of yours. The game is finished and a winner may be declared when all controllers have the same color.

On the technology side, we've decided to use UWB (ultra-wideband) network chips to do precise location tracking, which we need to discern which controller is actually closest to the current one, and combined with accelerometer data, we can accurately identify the team of the controller which most probably pushed this one.

* ### Last One Standing

Random controller glitter in intervals between 2 and 50 milliseconds as flashes of color or cool white, intensifying its rate until at some random point, the game is started and all controller turn green to initiate the first round.

People start moving now, slowly, to avoid turning their own LED red, and move towards other participants to try to move their lights in just the right way to make them red.

Alliances may form and the game takes its course.

The last light to turn red may then be declared as the round winner.
