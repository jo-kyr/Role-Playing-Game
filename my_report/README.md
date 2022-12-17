# Lesson: Digital & Serious Games

### First and Last Name: Kyriakou Ioanna
### University Registration Number: dpsd18058
### GitHub Personal Profile: jo-kyr
### Digital & Serious Games Personal Repository: https://github.com/jo-kyr/Role-Playing-Game
### Game Link: jo-kyr.github.io/Role-Playing-Game/

# Introduction


# Summary


# 1st Deliverable

#### Initial Settings
Following the instructions on the main page, I made a new fork of the Role Playing Game repository and activated GitHub Pages, so I can later publish my game there.

#### Getting Started
After setting up a new project in Unity, I started following the tutorial Ruby's Adventure. I made a new scene, imported my own character Neko and added basic motion through a script.

![getting_started](https://user-images.githubusercontent.com/97399069/201430416-789538cd-41f0-44ba-ba67-a90d21b9daf3.png)

#### Character Controller and Keyboard Input
Next, following the tutorial, I altered the script so that the player can control Neko through the keyboard arrows.

![neko_walking_test_Trim](https://user-images.githubusercontent.com/97399069/201431527-5386e8a0-b1b2-4779-9541-d4e99a7b64b6.gif)

#### World Design - Tilemaps
In order to built my own level, I searched on the Unity Asset Store for a tilemap set. I found one that I liked and added what I needed to my project. 

![assetstore](https://user-images.githubusercontent.com/97399069/201432013-36069f4d-cd14-45a7-9a33-8914613bde0c.png)

Following along with the tutorial, I created two tilemaps; one for the walls and one for the grass. This helps layer the tiles the way I wanted. Lastly, I created another layer for the props, which I imported from the asset store.

![walls](https://user-images.githubusercontent.com/97399069/201433158-8410f2a9-5b6f-41fc-b781-1889f0034e25.png)
![grass](https://user-images.githubusercontent.com/97399069/201433167-fbac7337-de25-4ff3-bd01-d773b7032483.png)
![objects](https://user-images.githubusercontent.com/97399069/201433182-c73a174e-75c8-4ac0-a45b-25934e94c19e.png)

#### Build, Run, Distribute
In order to share the game, I downloaded the WebGl platform and build the main scene. Next, I uploaded the Build, Template Data and index files to GitHub.

![neko_final_Trim (1)](https://user-images.githubusercontent.com/97399069/201435508-2f7c65aa-51a3-4509-a2f5-a038d46b63c4.gif)

# 2nd Deliverable
Before continuing with the rest of the assignment, I decided to make a new, larger level, so that the new elements will not overcrowd the game.

![level](https://user-images.githubusercontent.com/97399069/208247949-f995e7b3-5987-4e9a-8211-9a7b4c57e142.png)

#### Blocking Movement
The pack I imported already had colliders for most of the props. Following the tutorial, I added tilemap colliders to the walls so the player won't be able to walk through them. Lastly, I added a box collider and a rigidbody2D to the player sprite. After sorting everything in layers and ajusting Neko's script, the player can now move correctly within the world. (Images are from previous build.)

![wall_colliders](https://user-images.githubusercontent.com/97399069/201434295-84c56bc9-387a-4ac2-a712-887ff39db597.png)
![neko_box](https://user-images.githubusercontent.com/97399069/201434304-6460bc5f-6f46-443f-bcc2-bdc7522f612f.png)
![controller2](https://user-images.githubusercontent.com/97399069/201434319-86c7ff62-ab7c-400a-81f4-5cd472631a2e.png)

#### World Interactions - Collectibles
After deciding on what the player will be able to collect, I made some simple sprites to correspond to each category: health, speed, pink bullets, purple bullets. I followed the Ruby tutorial for the health system and collectible, then applied the same technique to the rest. At the start of the game, health and speed are at the maximum level - meaning the player can't pick up extra - and the bullet ammo is zero.

![collectibles](https://user-images.githubusercontent.com/97399069/208247960-a074849f-d6db-4656-9462-c58bbe4b4120.png)

https://user-images.githubusercontent.com/97399069/208248916-8e80e98b-c3f7-48ac-9160-8425abd256d5.mp4

https://user-images.githubusercontent.com/97399069/208248940-786a9a08-cbed-4dca-8215-8872027276ab.mp4

#### World Interactions - Enemies
After finding the enemy sprite I wanted to use, I imported it into Unity and added to the scene. After following the tutorial and making some changes to fit my game, the player now loses health when they make contact with the enemy.

![enemies](https://user-images.githubusercontent.com/97399069/208247995-5a09479f-4d0d-45d6-97d7-6c43e97f6e9a.png)

#### Sprite Animation
After studying the Ruby tutorial, I used the sprite editor to slice the player sprite sheet into individual sprites. Then, using the Animation window, I made an animation for each of the following: move left, move right, move up, move down, hit and idle. Lastly, I connected everything in the Animator. The enemy was also animated in the same way, with some additional code so that it moves back and forth on its own.

![neko_anim](https://user-images.githubusercontent.com/97399069/208247332-205896a9-2f7c-4628-9443-0ce6494591a6.gif)

#### World Interactions - Projectiles
This section required a lot of trial and error. I wanted the player to have two bullet types that they can switch between: pink and purple, with the purple inflicting more damage. The first step was to get the firing mechanism to work (mapped to "E"), according to the tutorial. There were some issues with the bullet not colliding correctly, but I managed to solve them by sorting the objects differently into layers. The second step was to enable the bullet switching (mapped to "Q"). After combining various online tutorials, I ended up using two switch cases. The first to actually switch the "active" bullet for the player, and the second to check which bullet is active and fire it. Lastly, I connected the pink and purple collectibles to the bullets, so that the player's ammo increases and decreases accordingly.

https://user-images.githubusercontent.com/97399069/208248976-a3c41957-16d9-4fc1-8618-6e10eda7b565.mp4

The code in this section - in combination with the collectibles - can certainly be simplified, so that will be a priority for the final delivery of this assignment.

#### Camera - Cinemachine
I had previously added the camera that follows the player during the 1st Deliverable. Cinemachine made this process very easy and straightforward.
![camera](https://user-images.githubusercontent.com/97399069/201434406-660cf47c-09d4-4eae-bf28-aacb88e3081d.png)

#### Build, Run, Distribute
In order to share the game, I built the main scene in WebGL and uploaded the Build, Template Data and index files to GitHub.

# 3rd Deliverable 
#### Visual Styling - Particles
#### Visual Styling - User Interface & Head Up Display
#### World Interactions - Dialog Raycast
#### World Interactions - Teleportation
#### Audio
#### Start Menu
#### Build, Run, Distribute

# Conclusions


# Sources

* https://learn.unity.com/project/ruby-s-2d-rpg?uv=2020.3
* https://pipoya.itch.io/pipoya-free-rpg-character-sprites-nekonin
* https://assetstore.unity.com/packages/2d/environments/pixel-art-top-down-basic-187605

