---
nav_sort: 2
src: /Getting Started/Creating an Achievement/Unreal Achievements.md
---

# Unreal Achievements

This tutorial assumes you have completed the '[Creating an Achievement](/Getting Started/Creating an Achievement/README.md)' tutorial and are ready to integrate the same functionality into your Unreal Engine Game. In this tutorial you will achieve the following: *Awarding an Achievement:*

Example code can be downloaded [here](http://repo.gamesparks.net/docs/tutorial-assets/UnrealAchievementsUassets.zip)

  * Execute a *GS LogEventRequest* and call the Event that will award the currently authenticated player an Achievement.
*Account Details Response:*

  * Create the *GSAccountDetailsResponse* node and *Break* the Account Details Response struct.
  * From the Account Details Response node retrieve the Achievements that the authenticated player has.
  * Print a message when the Achievement is unlocked.

*Testing the Achievement:*

  * Play a game that will award you an Achievement if the conditions are met.

### *Awarding An Achievement*

It's very simple to award an achievement to the Player using Unreal Engine SDK. All you have to do is call the Event that grants the authenticated player the Achievement, just like you did in the Achievements tutorial.

![l](img/UR/1.png)
 

### * Account Details *Response*

You can access many details about the *authenticated* player using *GSAccountDetailsResponse* node. This is where you can validate your player has received an Achievement, what currencies they own, etc.

![l](img/UR/2.png)

In this tutorial we will print out the authenticated players *Display Name* and the *Achievements* they have unlocked, as long as they achieve a new High Score, as that will be our trigger.

![l](img/UR/3.png)
 

### *Testing the Achievement*

The following image displays this in action. When we play the game and beat the High Score on the Leaderboard, we are notified about the High Score and all of our Achievements are printed out.

![l](img/UR/4.png)