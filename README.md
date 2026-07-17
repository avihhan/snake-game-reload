# Snake Game Reload

A responsive retro Snake arcade game housed in a red handheld console. Built as a dependency-free static web page and ready to deploy on Vercel.

## Play

- Press **Start** on the console or hit **Enter**.
- Steer with the virtual D-pad, arrow keys, or **WASD**.
- Press **Space** or the **B** button to pause or resume.
- Eat regular fruit for **+1 point** and one snake segment.
- A golden fruit appears after a random 5–15 regular snacks. Catch it before it disappears for **+5 points**.
- Avoid the screen edge and your own tail.

## Golden fruit timer

Its lifetime in seconds is `clamp(18 - 0.48 × (snake length - 3), 5, 18)`. Short snakes get more time; as the snake grows, the bonus timer gets shorter.

## High scores

The top five scores and their local date and time are saved in this browser's `localStorage`. Scores stay on the device and browser where you played.

## Run locally

Open `index.html` in a modern browser. No packages, build command, or environment variables are required.

## Deploy to Vercel

Import this repository in Vercel. Select the **Other** framework preset and leave the build command and output directory empty. Vercel will serve the root `index.html` as a static site.
