---
layout: post
title:  "Mobile App Dev Project 2 Milestone 2"
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
For this project, I will be creating a picross (nonogram) puzzle game. A nonogram puzzle is a picture logic puzzles in which cells in a grid must be colored or left blank according to numbers at the side of the grid to reveal a hidden picture.

## MVP (Minimum Viable Product)
The minimum functionality I want to be able to accomplish is as follows: 
  * To write a random picross puzzle generator to make the game replayable without hard coding lots of picross puzzles.
  * Users will be able to choose the difficulty by utilizing the slider to increase/decrease the puzzle size (from 3 to 8, subject to change).
  * Users will be able to enter a "safe" mode where they can toggle squares to be unclickable to prevent accidental mistaps.
  * Users will have a set amount of lives per level, scaled to difficulty.
  * Users will be able to scrub their current game at any time and restart.

## App prototype
<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="100%" height="700px"  src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Fproto%2FCHxpfjPtnmGTiDrscs5vkA%2FEndless-Picross%3Fnode-id%3D4%253A2%26starting-point-node-id%3D4%253A2" allowfullscreen></iframe>