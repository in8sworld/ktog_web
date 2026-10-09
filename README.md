# KtOG
This repo holds the source files for the KtOG website:

![](https://github.com/in8sworld/ktog_web/blob/master/20-sided.png)

[KtOG.in8sworld.net](https://KtOG.in8sworld.net)

KtOG is a simple dice-based combat game for 2 or more players created by Nate and his friends in the 1980s. You can read some more about the history of KtOG on the The Fighters page. In the game, each player attempts to ‘Kill the Other Guy(s)’ by ‘rolling to hit’ (using a 20 sided die), ‘doing damage’ (using a 6 sided die), and employing the various skills and spells at opportune times to win the game by reducing all other players to 0 ‘hit points’. Rewritten based on the KtOG discord bot to provide a way to play the game against up to three AI opponents.  Not as much fun as playing with real dice and real people!

## Change Log

### v261008201236
* switch combat log to DOM manipulation and CSS transitions for smoother flow
* add link to github on version number

### v261007193211
* Adds current HP in combat log (both for testing and clearer history)
* AI opponents can't be color red so they can't be confused with damage rolls
* Selecting four opponents is possible again for those who like punishment
* Heal gets animation rolls
* Major Fix: players can only cast one spell per round as per rules

### v261007065918
* Add a reset button to re-initialize the game at the bottom of the combat log so users don't have to refresh the page to do that.
* On the splash / start screen add a drop down for starting hit points so that users can pick short, medium and long game with hit points of 15, 20, and 25 starting hit points respectively

### v261006195018
* in the footer include tiny text for a version which is just the date and time that the file was last modified.
* Add to AI Strategy: Mighty Blow should be chosen after a successful hit but before damage is rolled.  AI strategy for determining whether to use Mighty Blow was discussed already in the chat log
* Modify Character card: Change the buttons to remove Punch so that there is only Attack and Disarm.  If a player is currently disarmed when they click the Attack button a pop-up confirmation should ask "you're currently disarmed, are you sure you want to attack bare handed?" and if yes, that attack follows the rules for Punch.  No player would ever use Punch unless disarmed.
* Log error in flavor text: in some of my flavor text (these little sayings only appear randomly based on some percentage and situation) I neglected to update {target} to ${cName(targetEnemy)} so the log shows {target} when it should replace it with the name of the player being targeted. 

