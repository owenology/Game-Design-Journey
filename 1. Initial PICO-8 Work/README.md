# GAME DESIGN JOURNEY

- [First Work](#first-work-22102026)
- [Learning the Map tool, and the player's interactions](#second-work-22102026)

### First Work: 22/10/2026

  * Made a game with very primitive movements (mostly learning how PICO-8 works using the terminal etc.)
  * The game was a red dinosaur that literally just moved around the screen based off Arrow Keys.
#### Tutorial used: 
  [SpaceCat's Beginner Tutorial](https://www.youtube.com/watch?v=LTMN5ItzzuA)  
  
#### My First PICO-8 Game — Red Dinosaur

<img src="pictures/first-picture.png"
     alt="My first PICO-8 red dinosaur game"
     title="My First PICO-8 Game"
     width="200">
  
### Second Work: 22/10/2026

  * This game was made to primarily understand the map system of PICO-8.
  * Learnt how to find the position of the player on the map, and based off this change how their character interacts with parts of the map.
  * Learnt to switch between sprites (provide visual queues for changing direction).
  * Found a cheatsheet online.
  
  #### Tutorials used:
    * [SpaceCat's Draw A Map Tutorial](https://www.youtube.com/watch?v=XjpZD4flViE&list=PLavIQQGm3RCmPt93jcg4LEQTvoZRFf9l0&index=4)
    * [SpaceCat's Find the Player's Postion Tutorial](https://www.youtube.com/watch?v=1m37s-SssTM&list=PLavIQQGm3RCmPt93jcg4LEQTvoZRFf9l0&index=4)
    * [SpaceCat's Map Interaction Tutorial](https://www.youtube.com/watch?v=cq11AB6Abaw&list=PLavIQQGm3RCmPt93jcg4LEQTvoZRFf9l0&index=5)

  #### What I learnt:
  * Maps has its own editor, and within said editor you make the map using 'parts' that you'd create in the same area that you'd make a sprite. Each 'part' is given its own number (for example '6'), however if you place multiple of the 'parts' it has the same number as one another (i.e. if I placed multiple of the number '6' part they'd all be read as '6' if the player is on it.).

  * I've learnt how to seen when the player / sprite goes onto a specific 'part' that you've made from the sprite editor, through using the 'MGET' command. Because of this, I've managed to make it so the player's speed changed based off what 'part' they're currently on - so I made a car that speeds up on the road, and stops when hitting a red sign.

  * I've also learnt to make bigger sprites (this time a car), as well as switching to other sprites on the press of a button (i.e. the left arrow key displays the sprite moving left, and the right arrow key displays the sprite moving right).

  <div>
    <img src="pictures/second-picture.png" width="300" alt="Car on road">
    &nbsp;&nbsp;
    <img src="pictures/car-rotates.png" width="300" alt="Rotating car">
    &nbsp;&nbsp;
    <img src="pictures/pico-8_cheatsheet.png" title="PICO Cheatsheet" width="500">
  </div>
