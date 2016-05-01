---
layout: 		softpost
title:  		"Stoppage Time"
thumb:      "st-thumb.PNG"
cover:      "st-cover.PNG"
release_date: 	2013-08-27
genres: [strategy,puzzle,sports]
colour:     "#84CBFF"
platforms:		[windows,osx,linux]
created_for:
  name:		"Ludum Dare #27"
  url:		"http://ludumdare.com/compo/ludum-dare-27/?action=preview&uid=9896"
source_code:
  name:		"GitHub"
  url:		"https://github.com/hndmrsh/Stoppage-Time"
screenshots:
  - url: "4.PNG"
    width: 1036
    height: 637
  - url: "3.PNG"
    width: 1036
    height: 637
  - url: "2.PNG"
    width: 1036
    height: 637
---
_Stoppage Time_ is a football (soccer) strategy game. (Note: Java 7 is required to play this game.)

Your club Youngtown FC are tied with league-leaders Central Park United in the last game of the season. There are only seconds remaining - can you help Youngtown score and win the league?

To score a goal, you must plan a single move, which will hopefully result in the ball hitting the back of the net. There are 4 commands available:

Move -- move the player to a position
Pass -- pass the ball to a position
Shoot -- shoot the ball to a position
Wait -- wait for 1 or more seconds

To add a command to the list, click on your player with the left mouse button, click the instruction you want to execute, and click the position on the pitch (or in the case of Wait, enter the number of seconds to wait for). Subsequent instructions can be added for the same player by clicking on the pitch while the instruction mode is active (e.g. click Move, then click multiple places on the pitch to plot a movement path).

To finish adding instructions, click the right mouse button (or click the right side of the screen). You must do this before you can select a different player!

To clear the instructions for a player, select the player and click the Clear command.

When you are ready to play your move, click the Play button. If you successfully scored, clicking will take you back to the main menu, where you can choose another scenario to play. If you failed, clicking will allow you to try again and adjust your instructions.

You can also press the R key at any time to retry the scenario. The Escape key also quits the game.

Now, go and help Youngtown win the league!

---

Fancy creating your own scenarios? All the scenario files are in ASCII format - all you need to do is copy the syntax from the existing .scn files (which should be fairly easy to understand)!
