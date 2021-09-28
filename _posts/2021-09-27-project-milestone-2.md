---
layout: post
title:  "Mobile App Dev Project Milestone 2"
---

The first project for my mobile app development course is to create a single view interactive iOS app. It can include apps that perform a calculation, respond to user input or selections, or respond to events in the app. We were encouraged to be creative and focus on design and user interaction.

### App Description
Originally, I planned to create a complementary color generator. I decided to switch to a a triadic color generator so there would be 3 colors total instead of 2. The user will input a color (in hexadecimal or rgb) and the app will calculate triadic colors.

### MVP (Minimum Viable Product)
The minimum functionality my app will meet is the following:
* Users will be able to enter a color using either hex codes or rgb sliders. 
* The app will calculate 2 colors from the user's input. 
* The app will display those colors and give a "preview" of a simple layout that utilizes those colors.

### Triadic color computation
* When I came up with this app idea, I planned to find an algorithm online to calculate triadic colors. I was unable to find anything that does exactly what I want, but I read up on some color theory to come up the following pseudocode algorithm: 

```swift
func calculateTriad(hex) {
    // get rgb values from hex (can also be used to update sliders after user input)
    red = hex[0:1]
    green = hex[2:3]
    blue = hex[4:5]

    // add and subtract by 85 (255 / 3), wrapping around if 0 or 255 is reached
    color1 = (add85(red), add85(green), add85(blue))
    color2 = (sub85(red), sub85(green), sub85(blue)) // add85 and sub85 deal with wrap around.

    return (color1, color2) // returns in rgb format
}
```

### Potential problems thus far
* I am having trouble adding complexity to my idea and am worried my app idea may be too simple. 
* It may be harder to implement a triad algorithm than I think it will be
### Prototype
* I created the following prototype with figma showing a simple version of my planned layout. 
<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Fproto%2F7lHdeYU4dRkmKiIpOeGhOK%2FTriad%3Fnode-id%3D5%253A41%26scaling%3Dscale-down%26page-id%3D0%253A1%26starting-point-node-id%3D5%253A41%26show-proto-sidebar%3D1" allowfullscreen></iframe>

### Screenshots
![triad screenshot](../../../img/triadScreenshot.png)