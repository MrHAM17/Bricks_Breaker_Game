# Bricks Breaker Game

This is "master" branch(main) of this repo; And presenting latest version (i.e, version no. 1.0) of the app.

It is the basic Desktop Game Application. Below, point by point complete detailed information is discussed.

## Chapter 1: Introduction

### 1.1 Motivation : 
Games are a fundamental way that humans interact and learn. They provide so many advantages for 
people of all interests and abilities.
 The main 
benefits of using computer games as learning tools, is related with problem solving, 21stcentury 
skills, integration of learning and assessment, collaboratives and interactivity, addressing cognitive as well 
as affective learning issues, and motivation for
 learning. Gaming is gaining a different level of attention 
not only from the youngsters but also from different age people.
 It is creating a virtual world where we can virtually live our life. Gaming has gained importance in 
Desktop application as well as in Android Application.
 
### 1.2 Need Of The Problem : 

As a computer science student, we’ve to learn game development because this field requires some skills that already we've and at the same time we can enhance them.

For a ‘game design’ it can mean “emotional engineering” or “largely communication” whilst for the other “everything that goes into a game is more or less game design”. On a more formal matter, many designers have gone extra miles to explicate their conceptions on game design.

Game development can considerably improve our imagination skills, designings kills and the ability to produce new things. For a game to attract attention, it should also be unique. The more the game is realistic, the more appealing and charming it is.

## Chapter 2: Problem Statement 
 
### 2.1 Working Flow Of System :  
We will implement a simple brick breaker game. We have layers of colored bricks and ball with 
which to break the layers. The player moves the paddle from left to right to keep the ball from falling.

The paddle doesn’t bounce the ball like a mirror, although it does so when the ball hits right in the middle. The closer the bounce take place to the left end of the paddle, a more significant left turn is added to an expected mirror bouncing.

A regular brick disappears when it’s hit by the ball, or breaks a little if it’s a bulkier brick. The basicuser interface may be similar to Figure 3.5. 

The output screen that will be displayed after the game is finished is the result to our developed game. The output that is displayed is the result to the developed program. The result shows that if a user completes the game completely the output pops out as VICTORY but if the user could not break all the bricks the output screen displays the Game Over pop out. The victory screen looks like Fig 3.4

### 2.2  Software Implementation :  
- 1. Paddle control :
     
     The paddle will be controlled by a mouse. The mouse’s moving to left or right will 
     correspond to the paddle’s movement. The moving speed will also relate to how fast we 
     move the mouse. By clicking on the left key, the paddle can launch extra balls as bonus 
     in higher level rounds.  

     Software will be used to keep track of the current status of the paddle, to see if it’s 
     under special status, like elongated, shortened, multi-ball launching, or fireball 
     launching (fireball can destroy all bricks in its trajectory). 
 
- 2. Bouncing ball :
     
     Software will be used to assigning new locations of the ball as the ball bounce around
     walls (edges of the screen), bricks and paddle. When the angle of incidence changes, the
     angle of reflection changes too.
  
     We will also need a status tracker to see whether the ball is in regular status or fireball status. Also, we implement the game with player have multiple lives.

 - 3. Bricks :
      
       For each brick, the software will have a status tracker. The tracker will record how many breaks needed to break a specific brick (different types of brick may need 1 or 2 or 3 times of breaking before they are destroyed), what special effect they have and when to release, and to display or not (remaining or destroyed).
 
 - 4. Score counting :

      Software will count for the scores and calculate the bonus points gotten by how many bricks broken in a row and other effects. The score will be displayed on the up right

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%202.1.jpg?raw=true)


## Chapter 3: Implementation

Prototype Model :

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%203.1.1.png?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%203.1.2.png?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/FIg%203.2.1.jpg?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%203.2.3.jpg?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/fig%203.2.4.jpg?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%203.2.5.jpg?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%203.2.6.jpg?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%203.2.7.jpg?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%203.3.1.jpg?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%203.3.2.jpg?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%203.4.1.jpg?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%203.5.1.jpg?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%203.6.1.jpg?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%203.6.2.png?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%203.6.3.png?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%203.6.4.jpg?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%203.7.1.jpg?raw=true)

![](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/2.%20Rough%20Work%20&%20Data/Used%20Images/Fig%203.7.2.png?raw=true)


## Chapter 4: Conclusion

### 4.1. Tech Stack :

-  **Developer:** Java, Apache-Net-Beans

-  **Client:** Smartphone with minimum 2GB RAM,  minimum API level of 21


 
###  4.2 Conclusion : 

The major aim of this project is to increase the problem-solving skills. The project aims to 
create a 2D game in pc is successful . Where users can access the game with ease. In this we 
learned how java is used in game development and in other applications. We have discussed 
about how brick breakout game is developed in java. 
 
Today many games are being produced in market. But this game is a new and a better version 
of a classic popular game which will increase the curiosity and eagerness among the users. 
Many action games are available today in market, but they are lacking in problem solving 
skills. 
 
So, concluding our project, the Brick Breaker Game demonstrated our learning and new found 
expertise in Verilog coding, the understanding of basic NetBeans IDE, basic Java 
Programming Language, Teamwork & all, How to handle a real life project, And many more 
things; Also last but not the least i.e. solution for our aim of the project.

### 4.3 Future Scope : 

The scope of the project is to develop a PC based 2D Game The programming language 
which will be used to build this game is C and opengl. The game will be influenced from 
Brick Breaker; the game will have space background and theme. Asteroids, Meteorites will be 
present as background of the game. The ball in the game is considered as a comet. 
 
First the player has to move the board which will be situated at the bottom of the screen and 
there will be a ball which will bounce after it comes in contact with the board and hit the 
bricks. Once all the bricks are destroyed, the level will be completed. 
 
There is only one level in the game at this point. There will be three life lines which is given 
to the player when the ball does not come in contact with the board. Standard of Each 
level will be increased with increase of number of bricks in each level. The board will move 
horizontally and will be controlled by the keyboard

## Documents

Project Report

![PDF](https://github.com/MrHAM17/Bricks_Breaker_Game/blob/master/1.%20Project%20All%20IMP%20Docs/Java%20Lab%20Project%20Report.pdf)

For more details,
Kindly Check the 1st folder of this repo i.e, "Prject All IMP Docs"



## Installation

Install my-project with:
- Apache NetBeans



## Reference:

- TEC, University of Mumbai, Mumbai, India  
  “PC Based 2D Game Design”, May-June-2021

- Stanley College of Engineering and Technology for Women, Hyderabad,

  “GLOBAL JOURNAL OF ENGINEERING SCIENCE AND RESEARCHES, BRICK 
  BREAKOUT”, 2018


- http://www.cs.columbia.edu/~sedwards/classes/2019/4840-spring/designs/BrickBreaker.pdf

- http://web.mit.edu/6.111/www/f2013/projects/jabbott_Project_Final_Report.pdf


- Youtube
   - https://www.youtube.com/watch?v=KED9ZTO4mhg
   - https://www.youtube.com/watch?v=gPiahyf70ds
  
- LinkedIn 

- Github 
