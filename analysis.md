# Analysis

## Defining The Problem

### Project outline

My project will consist of a 2D pixel-art survival platformer, an arcade which uses a predetermined set of rooms and enemies that the user will have to navigate through. The game is going to use a fixed camera around each room, which the user can navigate accordingly by using the X and Y axes on-screen. 

The overall goal of this game is to reach a high core by killing randomly generating enemies, and defeating entire waves of them. The user will also be able to collect an in-game currency, which can be exchanged upon death for permanent buffs to each player character. High scores will be saved under the user’s inputted username in a score table all users can view. 

This game will use simple keyboard controls, such as the A and D keys for simple left/right movement, the SPACE key to jump, the W and S keys to aim upwards or downwards, and the SHIFT key to slash with the sword. Having a relatively simple and recognisable control layout could provide younger or less experienced players with a user-friendly interface. This in turn makes my game available to a wider variety of target audiences.

### Stakeholders

My game is a 2D arcade platformer, designed to be a pick-up-and-play game, demanding less dedication towards the game strategy-wise, so is aimed at a more casual user group, being easy to learn and play. 

Personally, I am a great fan of 2D fighting platformers, so this game naturally appeals to me. Many other members of the gaming community appreciate such games, a chief example being Super Smash Bros. and Dead Cells. As such, my game would fit in with those stated above, thus would also be targeted to players such as myself.

### PEGI Rating

The official website classifies their 7 rating as: “Game content with scenes or sounds that can possibly be frightening to younger children should fall in this category. Very mild forms of violence \(implied, non-detailed, or non-realistic violence\) are acceptable for a game with a PEGI 7 rating.” 

Therefore, my target audience will be around the 7+ range, as I believe that although violence will be present, the graphical representation of my game, which uses pixel art, will not be graphic enough to frighten or negatively influence younger children, therefore will not fall into or above the PEGI 12 category. Furthermore, my game requires a frequent use of reflexes and a high reaction time. A younger audience, such as children under 7, may find it hard to keep up with the action on screen, so will not benefit much from playing it.

## Justification of Computational Methods Used

### The Need for Computational Methods

Computational methods would be ideal to create my project for several reasons: 

* My project is a game which simulates platforming and death, which is obviously not possible in a real-life context, hence the need for a simulation via computational methods.
* The user’s high scores can easily be saved and displayed on the main menu, as a program could be run by the computer to collect data about the player’s current score, and output this for any user to see, making the user interface more accessible and friendly. 
* The player can easily control the events of the game, by using inputs on a controller/keyboard to make the character take certain actions ingame. This can be done by the computer constantly checking for inputs, and running the appropriate code to give the desired outcome. 
* The game could also follow certain rules that the player does not necessarily know, such as the fall speed, enemy health stat or other variables and functions. This creates a more immersive experience by allowing the computer to process all the required data behind the scenes of the game, so that the player does not have to worry about any complex algorithms, and focus on enjoying the game. 
* Graphical representation is needed for my project, as the game needs to have a visual output for the player to see, in order for them to actually understand what the game is like. Computational methods would be ideal for this, as the software could just update the graphical output every frame to express the effect of what the player is doing. This is essential for the representation of the player character, objects, enemies, the landscape and other sprites.

### Thinking Abstractly and Visualisation

Abstraction is the process of removing unnecessary details from a program. Only important and essential aspects of the game world would be implemented into my game. This would include:

* Weather should be abstracted away completely, as it has absolutely nothing to do with my game, as it occurs mostly within a closed room, so is unnecessary to develop. ● Graphics will be abstracted down to basic sprite, by using a pixel-art theme throughout the game, which would cut down time on aesthetic design by a considerable amount, as I am not sure I can create visually appealing graphics in the development time I have to create the game. 
* Stage layout will be simple, with only the floor, the walls and a few platforms actually having colliders to interact with the player character and the enemies, which means I can safelyabstract away the background of the game as only aesthetics, meaning more development time spent on the more essential parts of my game. 
* Enemy behaviour will, via abstraction, use the technique of raycasting to search for the player character, and will likely use the A\* algorithm to calculate and take the shortest path to the player. This method is much quicker and viable than creating physical ‘eyes’ for every single enemy to search for the player character. 
* Rules relating to real life, such as fall damage, hunger and sleep, will not feature at all within my game, as I feel that their representation is useless within the boundaries of my game, as they detract from the experience and do not help in immersing the user into the action on screen.

### Thinking Ahead

In order to have a structured and organised approach to developing my game, I should outline the inputs and outputs needed for my game to run, as well as how they affect my game as a whole. 

For example, my inputs would include the WASD keys for movement and the SHIFT key for slashing with a sword. These inputs will remain consistent throughout the entirety of my game, and will not be affected at all as the game changes, providing an easy-to-use interface for the game’s user. Furthermore, outputs need to be specified early on, such as my player character’s position in the game world, and any values that the player needs to be aware of \(amount of currency, health etc.\), so that the user can understand what is going on in the game and how their inputs will affect the above.

### Thinking Procedurally & Decomposition

Decomposition is the process by which a larger, more complex task is broken down into more simple, easy-to-manage tasks. This is key in ensuring that I focus on one part of the game at a time, and completely finish one section of the code before starting to code another. Furthermore, some elements of my code \(eg. enemy deaths, increasing the amount of currency held\) will be the same, so I can bundle each of these into reusable program components, that I can use frequently throughout my code without wasting extra time rewriting each component, or making unnecessary errors that I could easily avoid.

### Thinking Logically

Throughout the course of the game, the player should be able to make free decisions about what action to take if multiple options are presented to them. The program must be able to make logical decisions to accommodate all choices the player makes throughout the course of the game, as well as making enemies react to the player’s presence, and keeping track of player stats in the background. The player will be presented with a variety of options to choose between as the game progresses.

* A player on the title screen should be able to decide what name they choose to save their progress under, which then displays their high score on a table in the title screen. The program must be able to accept all inputs for a name, and display the correct stored name as well as the relevant score that player got, as well as the total currency that player has accumulated.
* In the shop, the player will be able to buy certain upgrades for their character, of which more than one will be available at the same time, thus the program needs to be capable of handling any decisions made by the player in any order, and store these under the correct player.

The software itself must also be capable of making decisions regarding the game as it runs.

* The program should be constantly checking for valid external inputs from the game’s user \(eg. WASD keys to move, SHIFT to use the sword...\), and ignoring those that should not be accepted. 
* For the enemy movement, the program must be able to detect whether an enemy has ‘seen’ the player, and what actions it will take to move towards them. Whether or not to run a path algorithm to travel to the player character should depend on the distance between the player and the enemy, which the program should be constantly comparing while the game is active.

### Thinking Concurrently

When the game is running, several different tasks need to be carried out concurrently, meaning that multiple instructions are executed at the same time. This must be used for the following reasons:

* Sound effects need to coincide with the relevant interaction in-game \(eg. a slashing sound when the player’s sword is swung\), so as to quickly present the reader with easy-to-understand user feedback on what actions they have taken and create an environment closer to real life. 
* Player and enemy movement must occur at the same time in order to provide a more fluid and engaging player experience, as having the player and enemies taking turns to move would slow the game down significantly, which is not at all a desired outcome for a fast-paced game. To solve this, I could update sprite movement every frame, to simulate simultaneous movement

## Research

I have carried out research on games which present similar solutions to the problem I have set myself:

### Hollow Knight

![The UI only shows health, currency and mana without using the menu.](.gitbook/assets/maxresdefault.jpg)

#### Overview

A metroidvania made by indie developer Team Cherry, Hollow Knight is a two-dimensional platformer designed around exploration and combat, where the player explores a large, predetermined map. This game implements action and platforming elements, as well as a simple attacking system, which although limited, is still engaging and fun to use. It has been released on all major consoles, such as PC, Xbox, PlayStation and Nintendo Switch.

#### Controls

Hollow Knight’s main character is fully controlled by the player, with moving being bound to the arrow keys, and attacking, inventory usage and abilities \(eg. spells\) are all bound to the left side of the keyboard \(ASDF and ZXCV keys\). These controls can be freely remapped at any point. The character moves along the x-axis, and can jump along the y-axis, although is bound to these as this is a 2D game.

#### Story

Hollow Knight is a very story-driven game, with the main character following a vaguely predetermined route through the world as they try to find out more about the lore surrounding the game world. The enemies and bosses in the game all have a backstory to them being there, and even the main character has a backstory and purpose in the game world, which the player will eventually learn more about as the game progresses.

#### World Design

The world that Hollow Knight is set in is predetermined, but features many biome-like sub-areas with individual environments, enemies, bosses and soundtracks to create an immersive atmosphere, which makes the player feel as if they are actually in that specific environment. The platforms and backgrounds of the game constantly follow a specific colour scheme and texture to further represent the biome the player is currently exploring, which gives an aesthetically pleasing experience.

{% tabs %}
{% tab title="Features I Found Useful" %}
| Feature | Justification |
| :--- | :--- |
| 2D Side-Scrolling View | Having a side-on view means that the player can easily judge enemy distances, and respond to these accordingly. This also allows players to judge distances to make jumps and attacks. |
| In-game currency | Having a currency that the player obtains from killing enemies gives the player another motive to play the game other than getting a high score, such as buying upgrades in the shop. |
| An in-game shop | Being able to exchange currency for character upgrades means the player can feel rewarded for playing the game, adding more depth to the experience instead of limiting gameplay to getting a high score. |
| Boss fights | Having boss fights helps to break up the flow of the game, adding diversity to the types of enemy the player will fight. |
{% endtab %}

{% tab title="Features I Did Not Find Useful" %}
| Feature | Justification |
| :--- | :--- |
| Complex storyline | I believe that a combat-oriented arcade game does not need a storyline as complex as that of Hollow Knight , a mostly lore-driven game, as it will most likely not provide any enjoyment or understanding to the player, and detract from the action. |
| Massive map | My game will occur mostly in box-stages with platforms, so a big game environment is completely unnecessary for my project, as it will remove focus from the combat and enemies. |
| Exploration | The map will not have any secret rooms or similar, as the focus of the experience is to engage in combat, not world navigation |
{% endtab %}
{% endtabs %}

#### Features I Find Useful For My Game

| Feature | Justification |
| :--- | :--- |
| 2D Side-Scrolling View | Having a side-on view means that the player can easily judge enemy distances, and respond to these accordingly. This also allows players to judge distances to make jumps and attacks. |
| In-game currency | Having a currency that the player obtains from killing enemies gives the player another motive to play the game other than getting a high score, such as buying upgrades in the shop. |
| An in-game shop | Being able to exchange currency for character upgrades means the player can feel rewarded for playing the game, adding more depth to the experience instead of limiting gameplay to getting a high score. |
| Boss fights | Having boss fights helps to break up the flow of the game, adding diversity to the types of enemy the player will fight. |

#### Features I Don’t Find Useful For My Game

| Feature | Justification |
| :--- | :--- |
| Complex storyline | I believe that a combat-oriented arcade game does not need a storyline as complex as that of Hollow Knight , a mostly lore-driven game, as it will most likely not provide any enjoyment or understanding to the player, and detract from the action. |
| Massive map | My game will occur mostly in box-stages with platforms, so a big game environment is completely unnecessary for my project, as it will remove focus from the combat and enemies. |
| Exploration | The map will not have any secret rooms or similar, as the focus of the experience is to engage in combat, not world navigation |

