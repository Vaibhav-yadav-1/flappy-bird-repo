How We Made Flappy Bird Game –


1.	Game Board:
First, we created a canvas of size 360x640. Then, we added images for the background, bird, and pipes to make the game visually appealing.


2.	Controlling the Bird:
a)	We positioned the bird at the start of the screen (near the top-left).
b)	When we press the spacebar, the bird jumps up by setting a negative vertical velocity.
c)	If no key is pressed, gravity pulls the bird down continuously, simulating free fall.


3.	Making Pipes Move:
a)	We generate new pipes every 1.5 seconds at random vertical positions to keep things unpredictable.
b)	The pipes move left across the screen, creating the illusion that the bird is flying forward.


4.	Scoring System:
a)	When the bird successfully passes through a set of pipes, the score increases by 1.
b)	We give 0.5 points per pipe, and since each set has two pipes (one on top, one on the bottom), passing both earns 1 point


5.	Game Over Logic:
a)	If the bird hits a pipe or falls off the screen, the game stops.
b)	After a game-over, pressing the spacebar again restarts the game by resetting the bird’s position, clearing the pipes, and resetting the score to 0


6.	Collision Detection: We check if the bird’s position overlaps with any pipe. If there’s an overlap, it means the bird has crashed, and the game ends.


7.	Using Timers to Run the Game Smoothly:
a)	We run a game loop 60 times per second to move the bird and pipes smoothly.
b)	Another pipe placement timer ensures that new pipes appear every 1.5 seconds to challenge the player.

How to Play:


     1.	Press the spacebar to make the bird jump.

     2.	Pass through the gaps between the top and bottom pipes to score    points.

     3.	Avoid crashing into pipes or falling off the screen.

     4.	Game Over:
     i.	If the bird collides or falls, the game stops.
    ii.	Press space again to restart the game from the beginning.



Controls

Spacebar:
     i.	Makes the bird jump.
    ii.	Also restarts the game after a Game Over.



Prerequisites
     i.	Java Development Kit (JDK) installed on your system.
    ii.	Any Java-compatible IDE (like IntelliJ IDEA, Eclipse, or NetBeans) or the ability to run Java from the command line/terminal.



How to Run the Game
     i.	Download or clone the project files.
    ii.	Open the project in your preferred IDE or navigate to the folder using the terminal.
   iii.	Compile the code using:



How to rum the code:

i.	javac FlappyBird.java 
ii.	java FlappyBird.java



