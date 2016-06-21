---
src: /Tutorials/Real-Time Services/README.md
---

# Real-Time Services

## Introduction

Welcome to our series of tutorials on GameSparks Real-Time services SDK. These tutorials are intended to give you an introduction to our Real-Time SDK, how it works, and to provide you with a useful example on how our Real-Time might be implemented in a multiplayer game.


## What Are Real-Time Services?

Our real-time services provide a network communication layer which has the ability to send and receive data in real-time. Here are the main points:

* **Designed for Multiplayer Contexts.** Our real-time services are intended for use in multiplayer networked games where player and game-data should be sent and received as quickly as possible.

* **Host Server Support for Player vs. Player (PvP) Model.** We use a PvP model for our network programming. However, we use a host server to relay communications between players. This allows our services to support a higher number of players than traditional PvP models, as well has giving you the option to host games in the regions of your choice to reduce latency issues.

* **Lightweight and Flexible SDK.** Our real-time SDK is very lightweight, giving wide flexibility on what data you send and how you wish to send the data. The benefit of this is not just to give the developer control over what is sent and received, but also to keep the packets as small as possible which makes transmission much more efficient.

The tutorials in this section cover:

* [Setting Up Real-Time Matchmaking](/Tutorials/Real-Time Services/Setting Up Real-Time Matchmaking.md) - Integrating the real-time SDK into an existing GameSparks project in Unity3D and setting up a new real-time match through your game’s portal.

* [Real-Time Matchmaking & Player Lobby](/Tutorials/Real-Time Services/Real-Time Matchmaking.md) - Using the GameSparks matchmaking services to match players of a certain skill level.

* [Real-Time Chat Services](/Tutorials/Real-Time Services/Implementing Real-Time Chat Services.md) - Once a real-time session has started from the match setup in the lobby, how to start sending and receiving packets to build an real-time chat service.

* [Multiplayer Game Example](/Tutorials/Real-Time Services/Real-Time Game Example.md) - To demonstrate the real-time services, this tutorial shows you how to create a very simple multiplayer game. This example will have networked objects moving around, firing projectiles, and sending and receiving information between each player to update each other’s game-objects.

Each tutorial will have an accompanying video tutorial you can follow along with, as well as downloadable examples of the finished project at the end of the tutorial.

**<< ARE WE PLANNING TO DELIVER THESE VIDEOS? >>**