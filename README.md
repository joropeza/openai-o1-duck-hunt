# openai-o1-duck-hunt

Coding with ChatGPT using OpenAI's o1 model to make a Duck Hunt game

## The Prompts

### Prompt 1

Let's make a browser-based game using a single-page HTML file and JavaScript. The game will be played in a <canvas> that fits into an 800 max-width div. Follow these instructions:

1. Environment & Setup
    - Use a single HTML file with an 800 max-width div and a <canvas> that resizes to fill it.
    - Write all code in a <script> tag.
2. Scene & Floor
    - The scene floor is a cartoon marsh represented by green grass.
    - Several trees in the background.
    - Render a simple sky background (gradient).
3. Gun (Mouse-Aim & Fire)
    - The mouse pointer should be replaced by a crosshairs when hovering over the canvas
    - Clicking the mouse button should cause the crosshairs to flash
4. Code Structure
    - Use ES6 classes for Gun, Shell, Duck, etc.
    - A main loop runs the game.

### Prompt 2

Make the total canvas height be equal to its width. Then let's build out that duck class. Use this image <https://seeklogo.com/images/D/Duck_Hunt-logo-8044A0A3B6-seeklogo.com.png> of a duck flying to the right. Reverse the image if the duck is flying to the left. One duck should enter the screen at a random height every 3-7 seconds. The duck should enter at one edge of the screen and move fairly quickly towards the other side of the screen.
