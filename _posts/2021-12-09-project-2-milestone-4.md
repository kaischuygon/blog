---
layout: post
title:  "Mobile App Dev Project 2 Milestone 4"
---

The second project for my mobile app development course is to create a single view interactive Anroid app using Android Studio and written in Kotlin. 

The project requirements are as follows:
- Think of a creative idea or concept
- Focus on how the design and interactivity flows for the user
- The scope of your project should be larger than that of a lab
- Your app should use a constraint layout for an adaptive layout for different device sizes including portrait and landscape orientations
- Your app should be complete with a custom theme and launcher icons
- Your app should use string resources for text in the user interface

## App description
For this project, I decided to create a Picross (nonogram) puzzle. A nonogram puzzle is a picture logic puzzles in which cells in a grid must be colored or left blank according to numbers at the side of the grid to reveal a hidden picture.

The main feature of my MVP was that each puzzle would be randomly generated, enabling users to have an "endless" supply of puzzles. I decided to avoid common features of other picross apps on mobile devices such as progress saving, lives, ads and a pre-determined puzzles. I wanted the app to be a quick experience you could spend anything from minutes on to hours. 

## Creative Approach
The most creatively challenging aspect of this application was making the layout visually appealing enough to make users enjoy the application without adding too many visual elements that would distract from the point of the app. I thought about making custom buttons and theming the application more but ultimately decided to go with a simple dark material design theme. I used the [material design color tool](https://material.io/resources/color/) to create the `colors.xml` file that is used throughout the application. I experimented with various colors and liked the look of a dark navy blue background with magenta accents.

## Technical Approach
This was definetely the most challenging aspect of the final MVP. I ended up creating a seperate class for implementing all game logic called `Picross.kt` that stores 2 2D arrays, one representing the current game board and another representing the solution, both as `1`s and `0`s, and all the functions associated with running the game. I placed all this in a seperate class so it would be easy and efficient to start a new game and to not confuse the tile board with the boolean board. 

The actual logic behind randomly generating puzzles was a bit more involved than I originally thought. It is pretty easy to make a game board and generate hints, but it is extremely difficult to ensure that a puzzle has a unique solution. As the app currently stands, it is possible but very unlikely that a puzzle is encountered that has multiple solutions. Only one solution will work however. This is a problem I will try to fix but the game is playable as is. If you happen to run across a puzzle with multiple solutions you can press the new game button at the bottom to generate another puzzle that (hopefully) does not have the same problem. 

## Time allotment
I started this project fairly early and slowly worked on it throughout the course of 2 weeks. The most time consuming aspect was creating the tile board. I tried to create it programatically at first so that users would be able to change the dimensions of the board and in turn increase/decrease difficulty. This is very difficult in android and I could not find a way to do it that would work with the way I was calling the `onClick` function that would toggle the button colors. In order to implement different size boards I will probably have to do some reformatting of my app's XML and `MainActivity.kt`. Other than that, everything went pretty smoothly and I was able to get a version of my original idea I am happy with. 

## Things that went well
My idea to create a seperate class for just game logic was definetely the right move. It made creating new games very easy, I just had to call the class constructor again once a game was over and everything reset.

## Things that did not go so well
The way the tiles change colors is not ideal. The IDs of the tiles are hard coded and are there for not modular for different size game boards.

## Things I'd change going forward
I would define MVPs that are more focused. My MVP for this application seemed simple when I came up with it but once I started I realized that I would not be able to accomplish all of it with the time allotted. 

I want to take the time to make the board resizeble and implement a unique solution check for puzzles. A classmate suggested a timer and I think that would also be a great addition. More variety in theming would be easy to implement and would make the entire app more replayable, _Centipede_ style. Finally, cleaning up code and making the app more efficient would probably not be a bad idea. 