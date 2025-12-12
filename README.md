# Ocean Battle Racing

**Ocean Battle Racing** is a fast-paced, 3D arcade racing game built entirely in a single HTML file using Three.js. Navigate treacherous waves, blast your opponents with broadside cannons, and race to the finish line without capsizing or crashing into rocks.

## Features

*   **Dynamic Water Physics:** Real-time wave simulation that affects boat pitch and roll.
*   **Combat Racing:** Fire broadside cannons (port and starboard) to sink rival racers.
*   **Procedural Tracks:** The race course is generated slightly differently each time.
*   **3 Difficulty Levels:**
    *   **Easy:** Calm waters, wider track, player speed advantage.
    *   **Normal:** Standard waves and competition.
    *   **Hard:** High waves, choppy water, narrow track, and aggressive AI.
*   **Destruction:** Boats can capsize from waves, sink from cannon fire, or be destroyed by collisions with rocks or other ships.

## How to Play

### Controls
*   **W / Up Arrow:** Accelerate
*   **S / Down Arrow:** Brake / Reverse
*   **A / Left Arrow:** Steer Left
*   **D / Right Arrow:** Steer Right
*   **SPACE:** Fire Broadside Cannons

### Rules
1.  **Stay on Course:** If you stray too far from the buoys, a 5-second disqualification timer begins.
2.  **Don't Sink:**
    *   Avoid hitting rocks or other boats (instant death).
    *   Don't let the waves flip your boat (capsizing).
    *   Dodge enemy cannonballs.
3.  **Win:** Be the first to cross the finish line.

## How to Download and Run

### Option 1: Direct Download
1.  Download the `index.html` file from this repository.
2.  Double-click `index.html` to open it in your default web browser (Chrome, Firefox, Edge, etc.).
3.  **Note:** An internet connection is required to load the 3D engine (Three.js) from the CDN.

### Option 2: VS Code (For Developers)
1.  Open the folder containing `index.html` in VS Code.
2.  Install the "Live Server" extension.
3.  Right-click `index.html` and select "Open with Live Server".

## Playability Evaluation

### The Good
*   **Visuals:** The water shader is surprisingly effective, creating a convincing ocean atmosphere with foam caps and depth color gradients.
*   **Physics:** The boat's interaction with the waves feels "floaty" and responsive. The risk of capsizing adds a layer of skill beyond just holding the "forward" button.
*   **Combat:** The ability to shoot sideways (broadside) encourages strategic positioning rather than just chasing the leader.

### The Challenge
*   **Difficulty:** The "Hard" mode is genuinely difficult due to the wave height. It requires careful throttle management to avoid flipping over.
*   **Punishing Collisions:** Hitting a rock or another boat results in instant game over. This is an "old school" arcade difficulty choice that rewards precision but can be frustrating.

### Technical Note
The game runs entirely in the browser using WebGL. Performance is generally smooth, but the vertex-displacement water simulation might be demanding on very old laptops or mobile devices.

## Development & Prompts

This game was "vibe coded" using **Gemini 3 Pro**. The entire codebase (HTML, CSS, and JavaScript/Three.js) was generated through natural language prompting.

### Prompts Used
Create a single-page app in a single HTML file with the following requirements:
- Name: Ocean Wave Simulation
- Goal: Display realistic animated waves.
- Features: Change wind speed, wave height, lighting.
- The UI should be calming and realistic.

... Gemini processing

Lets run this in Canvas

... Gemini processing

Now add a boat that we can watch be affected by the waves

... gemini processing

Now allow me to steer it and press something to push on the gas. There should also be the risk of capsizing which is the goal to avoid. that restarts the game

... Gemini processing

Lets make this all look so much more real!

... Gemini processing

Lets add obstacles to avoid (crashing restarts the game) there should be a path that is guided by boueys that help to keep the path and know which way to go, there are other boats racing and there is a start for our boat and and end location. There we identify if we came in 1st through 10th (the total number of boats that include ours). There should also be cannon with unlimited shots we can fire from the space bar that shoot from the sides of the ship to take others out and those boats have the same ability. This should be exciting! Also I notice our boat never capsizes, which it should if it is not driven well enough in those waves

... Gemini processing

I think they all start too close togehter, they are crashing immedietly. Also when restarting the game should allow focus back on the boat, when I click forward its like the boat is not selected and I end up falling behind immediely. A nice 3 2 1 start would be good. Also if you go outside the path too long it should tell you there are 5 seconds to get back inside the path otherwise you lose and restarts. Finally I think the wave high and choppoiness should be a setting "easy, normal hard" where you incrsase it and that way the player has new challenge levels. When the game initiates there should be a setting that lets you select it

... and that was it...

Have fun playing!