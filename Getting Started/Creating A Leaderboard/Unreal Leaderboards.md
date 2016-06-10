---
nav_sort: 2
src: /Getting Started/Creating a Leaderboard/Unreal Leaderboards.md
---

# Unreal Leaderboards

## Introduction

If you have followed the Portal [Tutorial](./README.md) for making an Event and a Leaderboard, then for this tutorial all you will need to do is call your Event. Here is a basic overview of what will be achieved through this tutorial.

*Gamesparks Message Listeners*

  * Creating a GS *MessageListeners* Component in your Game Mode class.
  * Retrieving the *OnNewHighScoreMessage* Event using the Listener.
  * Breaking the received message and printing out the name of the Leaderboard to the currently authenticated player.

*Calling the Event*

  * Call an Event that is linked to the Leaderboard.
  * Pass the SCORE value through to the Event.
  * Play the game and beat the High Score to receive feedback from the Service.

Example code can be downloaded [here](http://repo.gamesparks.net/docs/tutorial-assets/UnrealLeaderboard_Tutorial.zip)

## Setting up the Message Listener

First we'll need to create a *GSMessageListeners* component (located on the red bar on left) in the Game Mode. The GSMessageListeners component is an extremely useful tool which will allow you to intercept messages from the Portal to your authenticated player, then break them down and use them in your sequences. Here we're going to demonstrate the use of one message type interception by using the event *OnNewHighScoreMessage.* This can be dropped into the Event Graph after clicking the GSMessageListeners component and accessing its events (Green box on the right). Once we drop the Event in, we can break the message down and access data that is useful to us. For this tutorial we'll be retrieving the name of the leaderboard to inform the player which Leaderboard they have achieved a High Score on.

![l](img/UR/1.png)

## Setting up the Event Call

Once the Listener is ready, we can call the Leaderboard_Score event from anywhere we wish to upload the final score to. For this tutorial we have placed it right after our game countdown reaches zero and the points we collected during the game are uploaded to the Leaderboard. If a new High Score for is achieved for the currently authenticated player, a message will be sent to notify them. Now execute the Event that was previously set up on the Portal using *GS LogEventRequest*. You will have to pass in the *SCORE* attribute into the Event. In this instance we *Floor* our float score to round it off to the closest int and transform this value into an int. In this game example we are using *Floor* to transform our float value into an int value, then use the *Set Number* to set the value for the attribute.

![l](img/UR/2.png)

## Testing

Finally you can play the game. Here you can authenticate, play the game, and if you beat the High Score, you will receive a message saying you did so.

![l](img/UR/3.png)