---
layout: post
title:  "Mobile App Dev Project Milestone 4"
---

The first project for my mobile app development course is to create a single view interactive iOS app. It can include apps that perform a calculation, respond to user input or selections, or respond to events in the app. We were encouraged to be creative and focus on design and user interaction.

### App Description
For this project, I decidd to create a triadic color calculator. The user inputs a color (in hexadecimal or rgb sliders) and the app calculate triadic colors based off the input.

### MVP (Minimum Viable Product)
The minimum functionality I outlined my app would meet is the following:
* Users will be able to enter a color using either hex codes or rgb sliders. 
* The app will calculate 2 colors from the user's input. 

### Process
I am proud of the app I was able to create with the time I was given, but reflecting back there are definetely things I could improve on before the next project.
* Creative Approach
    * The hardest part creatively for me was definetely coming up with the concept of the app. My knowledge of iOS development definetely limited the app I could make but I think my MVP is a good starting point towards creating an app I could build upon as I continue learning app development.
* Tactical Approach
    * I first started my app by creating the layout of the app in a storyboard. This included adding all the visual elements as well as adding  constraints so the layout would work in multiple size screens in portrait mode.
    * I then added connected outlets and actions to the `ViewController.swift` and constrained the user's input to the values the app will be able to support.
    * Then I implemented the hex to rgb algorithm so that when the sliders update, the text input updated to match, and vice-versa.
    * I then implemented a the triadic color algorithm based off some color theory I read up on. I shifted the rgb values twice as follows:

    ```swift
    # First calculation:
    rgb = brg
    # Second calcuation:
    brg = gbr
    ```
    * Finally, I went back to the storyboard and added constraints to make the application responsive to landscape mode on multiple different screen sizes. 
* Time allotment
    * Most of my time for this project was spent on translating hex to rgb, largely because of my infamilarity with Swift. 
    * Another aspect of the project that took a long time was deciding on a algorithm to calculate triadic colors. There are multiple methods for doing this and I spent a long time trying to implement the first solution I found on Google which ended up being a lot more involved than it needed to be.
    * I was able to get the storyboard done fairly quickly by looking back on class examples.

### Reflection
* Things that went well:
    * I think that the implementation of the color calculate 
* Things that didn't go well:
    * I started the project too late to create a great UI, the app is definietely usable but lacks a unique UI.

### Priorities for future projects
* Focus on the UI a lot more, it's arguably just as important as the functionality of the application.
* Come up with a more creative app idea.