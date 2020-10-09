# Chapter 1: Designing a Game from Scratch

## Table of Contents
[TOC]

# I. Game concept
* **Preproduction:** create a development plan. Idea > Design > Develop

## A. Game idea

* **Game idea:** basic concept of game

  > Super Shooter will be a 3D game featuring a Futuristic Hero Soldier as the player character. The character must fight against Enemy Soldiers. These Enemies are intent on destroying our Hero's base and anyone that gets in their way, including our Hero. He will have a limited number of bullets he must keep track of.

## B. Input controls

* How will players interact with our game? VR, controller, keyboard/mouse?

* For our game:

  | Keyboard input    | Action           |
  | ----------------- | ---------------- |
  | Up arrow / W      | Move forward     |
  | Down arrow / S    | Move backward    |
  | Left arrow / A    | Move left        |
  | Right arrow / D   | Move right       |
  | Mouse movement    | Rotate character |
  | Left mouse button | Shoot bullet     |

## C. Winning and losing

* Win condition: when all the enemy waves have been defeated
* Lose condition: when either the Base life or the Hero's life is 0.

# II. Game characters

* Player character
* NPCs controlled by AI

## A. Hero

* Player character
* Needs idle, run, shoot animations

## B. Enemies

* Need to know how many, where they are placed.
* Control behavior through AI
* Need run, attack, and death animations

# III. Gameplay

 ## A. Game-world layout

* Start with basic schematic of environment

![image-20201009125958048](C:\Users\brand\AppData\Roaming\Typora\typora-user-images\image-20201009125958048.png)

* Consists of a few types of objects:
  * Wall: Impenetrable barrier preventing player from going outside play area
  * Door: Impenetrable, but serve as spawn position for enemies
  * Player start: starting position
  * Base building: wall, but needs to be protected.
  * Floor

## B. Starting condition

* Number of and placement of spawn points
* Number of bullets held by hero
* Placement of the base
* Need to track remaining waves, base health, and player health

## C. Ending condition

* If remaining waves == 0, player wins
* If player health == 0, enemies win
* If base health == 0, enemies win

## D. Point system

* Add points based on enemies killed

## E. HUD

* **Heads up display:** visual layer of information that is always present on the screen.

![image-20201009130540058](C:\Users\brand\AppData\Roaming\Typora\typora-user-images\image-20201009130540058.png)

# IV. The difficulty balance

* Too difficult: players get frustrated and give up
* Too easy: won't appeal to intended audience

## A. Difficulty questions to ask

### 1. General questions

* Should we have different levels of difficulty selectable by the player?
* What specifically will be different with each difficulty level?
* Should we have multiple game levels, each with an increased amount of difficulty?
* What specifically will be different with each game level?

### 2. Questions regarding enemies

* How many enemies should be spawned on each wave?
* At what distance should an enemy become aware of the Hero?
* How much damage should an enemy inflict on the player with each attack?
* How much damage can an enemy endure before it dies?

### 3. Questions regarding the player character

* How much life should the player have?
* How much damage will the player take from a single enemy attack?
* Should the character be able to outrun enemies?
* How fast should the player run out of bullets?
* How many bullets can the player have?

### 4. Questions regarding the environment

* How many attacks should it take for an enemy to destroy a base?
* What is the ideal max number of enemies spawned in a wave?
* Where should doors and bases be located in the game environment?
* How much damage should a bullet do?

## B. Implementation plan

* Answering these questions informs a lot of what the game will look like.
* If decide to implement one game level, but provide the user with three difficulty settings, a Difficulty Implementation Matrix might look like this:

![image-20201009131500640](C:\Users\brand\AppData\Roaming\Typora\typora-user-images\image-20201009131500640.png)

# V. Documentation

* Important to document everything. Helps explain vision to others, helps investors, helps make vision concrete.

## A. Game design document (GDD)

* "Basically the Bible of your game."
* Breakdown of all aspects with detailed documentation for each.
* There isn't really a standard format, or standard tools
* Sections:
  * Setting and introduction
  * Gameplay sections (crafting, quests, moving, etc)
  * Content sections (characters, story, world, etc)

# VI. Summary

* Need to think about a lot before starting
* Refer back to this chapter after brainstorming, but before developing.