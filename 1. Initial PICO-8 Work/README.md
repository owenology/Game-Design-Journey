<div align="center">

# PICO-8 Game Design Journey

</div>

<div align="center">
 
| # | Entry | Date | Focus |
|:-:|-------|:----:|-------|
| 1 | [First Work](#first-work) | `22/10/2026` | Basic movement |
| 2 | [Second Work](#second-work) | `22/10/2026` | Maps and player interaction |
| 3 | [Platformer](#third-work) | `23/10/2026 - ?` | Functions and 'physics' |
 
</div>

<br>

---

<details open>
<summary><h2 id="first-work">First Work:</h2></summary>

![Entry](https://img.shields.io/badge/Entry-1-FFD700?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Basic_movement-blue?style=for-the-badge)
![Made with](https://img.shields.io/badge/Made_with-PICO--8-ff004d?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)

📅 **22/10/2026**

  * Made a game with very primitive movements (mostly learning how PICO-8 works using the terminal etc.)
  * The game was a red dinosaur that literally just moved around the screen based off Arrow Keys.

<p align="center">
  <img src="pictures/other-media/first-work_0.gif"
       alt="My first PICO-8 red dinosaur game"
       title="My First PICO-8 Game"
       width="250">
  <br>
  <em>My first PICO-8 game: Red Dinosaur</em>
</p>
  <em>My first PICO-8 game: Red Dinosaur</em>
</p>

### Tutorial used: 
>  [SpaceCat's Beginner Tutorial](https://www.youtube.com/watch?v=LTMN5ItzzuA)  

<sub>[↑ Back to top](#pico-8-game-design-journey)</sub>

</details>

---

<details open>
<summary><h2 id="second-work">Second Work:</h2></summary>

![Entry](https://img.shields.io/badge/Entry-2-FFD700?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Maps_and_player_interaction-blue?style=for-the-badge)
![Made with](https://img.shields.io/badge/Made_with-PICO--8-ff004d?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)

📅 **22/10/2026**

  * This game was made to primarily understand the map system of PICO-8.
  * Learnt how to find the position of the player on the map, and based off this change how their character interacts with parts of the map.
  * Learnt to switch between sprites (provide visual cues for changing direction).
  * Found a cheatsheet online.


<table align="center">
  <tr>
    <td align="center">
      <img src="pictures/second-picture.png" width="250" alt="Car on road"><br>
      <em>Car driving on the road</em>
    </td>
    <td align="center">
      <img src="pictures/car-rotates.png" width="250" alt="Rotating car"><br>
      <em>Car sprite changing direction</em>
    </td>
    <td align="center">
      <img src="pictures/other-media/second-work_1.gif" width="250" alt="Car driving in the game"><br>
      <em>Car in motion (GIF)</em>
    </td>
  </tr>
</table>

### What I've learnt:
  * Maps has its own editor, and within said editor you make the map using 'parts' that you'd create in the same area that you'd make a sprite. Each 'part' is given its own number (for example '6'), however if you place multiple of the 'parts' it has the same number as one another (i.e. if I placed multiple of the number '6' part they'd all be read as '6' if the player is on it.).

  * I've learnt how to see when the player / sprite goes onto a specific 'part' that you've made from the sprite editor, through using the 'MGET' command. Because of this, I've managed to make it so the player's speed changed based off what 'part' they're currently on - so I made a car that speeds up on the road, and stops when hitting a red sign.

  * I've also learnt to make bigger sprites (this time a car), as well as switching to other sprites on the press of a button (i.e. the left arrow key displays the sprite moving left, and the right arrow key displays the sprite moving right).

<details>
  <summary><b>PICO-8 cheatsheet (click to expand)</b></summary>
  <br>
  <img src="pictures/pico-8_cheatsheet.png" title="PICO Cheatsheet" alt="PICO-8 cheatsheet" width="600">
</details>


### Tutorials used:
> [SpaceCat's Draw A Map Tutorial](https://www.youtube.com/watch?v=XjpZD4flViE&list=PLavIQQGm3RCmPt93jcg4LEQTvoZRFf9l0&index=4)
>
> [SpaceCat's Find the Player's Position Tutorial](https://www.youtube.com/watch?v=1m37s-SssTM&list=PLavIQQGm3RCmPt93jcg4LEQTvoZRFf9l0&index=4)
>
> [SpaceCat's Map Interaction Tutorial](https://www.youtube.com/watch?v=cq11AB6Abaw&list=PLavIQQGm3RCmPt93jcg4LEQTvoZRFf9l0&index=5)

<sub>[↑ Back to top](#pico-8-game-design-journey)</sub>

</details>

<details open>
<summary><h2 id="third-work">Third Work:</h2></summary>

![Entry](https://img.shields.io/badge/Entry-3-FFD700?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Functions_and_'physics'-blue?style=for-the-badge)
![Made with](https://img.shields.io/badge/Made_with-PICO--8-ff004d?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-In_progress-orange?style=for-the-badge)

📅 **23/10/2026 - ?**

* This game is being made to further improve my understanding of object interaction in PICO-8.
* Learned how to make a jumping and falling mechanic.

### What I've Learnt:

#### Code-related
* PICO-8 allows you to make multiple tabs with code on each tab.
* The variables / functions are universal between tabs.
* I've learnt how valuable functions are (they made the main tab so much easier to read).
* I've learnt how valuable Tables are. (I used a table to store the player's variables):
<details>
<summary><h4>Player Table Example</h4></summary>
```lua
	player = {
		sp=1,
		x=59,
		y=59,
		w=8,
		h=8,
		flp=false,
		dx=0,
		dy=0,
		max_dx=2,
		max_dy=3,
		acc=0.5,
		boost=4,
		anim=0,
		running=false,
		jumping=false,
		sliding=false,
		falling=false,
		landed=false,
	}
```
</details>

#### PICO-8 Physics-related

<sub>[↑ Back to top](#pico-8-game-design-journey)</sub>

</details>
