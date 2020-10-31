# INTREPID RIDER: The Game

## Description
Being a bike rider in a busy big city is an intrepid mission. The object of the game is to direct an intrepid rider through the crowded traffic. The player must avoid several vehicules to prevent our rider from dying tragically.

## MVP (DOM - CANVAS)
A driver that can move in 2 directions and has to be directed to avoid the incoming cars. The game is over when the player collides with one car. 
The game is won whenever the rider goes through all cars and the street is empty. 


## Data structure
1. index.html
2. main.js
3. game.js
4. player.js
5. vehicles.js
6. canvas.js

### 1. index.html file

### 2. Main file

- buildDom
- createStartScreen / removeStartScreen
- createGameScreen / removeGameScreen
- createGameOverScreen / removeGameOverScreen
- createWinScreen / removeWinScreen
- startGame / endGame

### 3. Game Constructor

**Properties**
- canvas
- ctx
- player
- name
- vehicles
- otherSide
- gameIsOver
- gameIsWon
- bonus
- loopCount
- timeScore
- pause

**Methods**
- start
- startLoop
- checkCollision
- checkOtherSide
- checkIfBonusWon
- checkTime
- win
- gameWon / gameOver
- printLives
- printTime

### 4. Player Constructor

**Properties**
- canvas
- ctx
- x position
- y position
- width
- height
- lives
- image
- direction

**Methods**
- draw
- move
- collidedWithObstacle
- collidedWithScreen
- catchedBonus
- removeLife
- addLife

### 5. Obstacle Constructor

**Properties**
- canvas
- ctx
- x position
- y position
- width
- height
- row
- speed
- direction
- image

**Methods**
- draw
- move

### 6. Bonus Constructor

**Properties**
- canvas
- ctx
- size
- x position
- y position
- image

**Methods**
- draw
- move
