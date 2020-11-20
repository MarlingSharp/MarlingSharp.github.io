# Analysis \(One-Page\)

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





