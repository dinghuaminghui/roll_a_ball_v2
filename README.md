# roll_a_ball_v2
Hello this is roll_a_ball version 2.0
Except the required change and additions, I have the following features this time:
1. Purple square traps to make you fail the game
2. Restart button to restart the game if you fail
3. Moving walls

1) Traps:
I created some flat squares and use trigger when ball is colliding with them. As long as trigger is activated, I set the ball's vertical position to be less than 0, and add a conditional in update to see whether the ball's current vertical position is below 0, then give out the lose game text. This also add a bit difficult to the game.

2) Restart Button
I created a button first. Then I write the script for restart game when clicking the button using SceneManager to load the using scene to restart the game. Then I put this button to be in player gameobject set it inactive until the fail text is out. So that if you fail you can click restart to challenge again.
PS: The reason that I don't put this button on winning situation is that I do not think it is meaningful to play it again if you already win XD.

3) Moving Wall
This one is easy. I just add a script to a random wall, and set a start position and end position. Using a bool flag, I can check whether it should move to one direction or the other. And if it is to one direction, i just update its transform postion with fixed number. So in this case, the wall will constantly move back and forth.
