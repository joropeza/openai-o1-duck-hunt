# openai-o1-duck-hunt

Coding with ChatGPT using OpenAI's o1 model to make a Duck Hunt game.

Each commit in the blame represents the code written by o1 after given the prompts below.

See the results here: [https://jonoropeza.com/2025-openai-duck-hunt/](https://jonoropeza.com/2025-openai-duck-hunt/)

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

### Prompt 3

Ducks should always appear in the upper third of the canvas. Also, make them fly at a random speed, not too fast, not too slow.

### Prompt 4

Let's introduce a distance dimension. Each duck instance should have a distance from the shooter between 30 feet to 200 feet. Choose a distance for each instance at random. Scale the size of the duck so that ducks that are further away appear smaller. Use the current size for ducks that are 50 feet away. Ducks that are 200 feet away should be much smaller.

### Prompt 5

Firing the gun by clicking the mouse button should fire a shell. Each shell should travel in a straight line. Shells travel at 1,000 feet per second. When the shell reaches the same distance as a duck instance that's currently on the screen, decide if there is a hit by determining if the shell is within a 100 pixel radius of the location of the duck. If there is a hit, console.log "hit!".

_Here I had to make my first correction:_

Shells should not linger. They should be deleted once they have travelled 500 feet.

### Prompt 6

_At this point, anything I prompted o1 to do next resulted in parts of the code being commented out like this:_

```
/**
 * (Other classes omitted for brevity, but identical to the previous code)
 * ...
 */
 ```

_Attempts to coach o1 to put it back together failed; we never returned to working code beyond this point, and so I decided to declare the experiment complete._
