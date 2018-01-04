# Avoid Bug Touch Water

## About
A simple, single-level Frogger-like game built in JS and painted onto an HTML5 Canvas. This project experiments with browser-based gameplay and light JS game engines.

## Getting Started
To start playing and tweaking the game:
1. check that you have a browser with full support for JS and HTML5 Canvas
2. download, clone or fork this repo
3. navigate to and open the root `index.html` with your browser
4. make changes to the code within the `./js` subdirectory to change game behavior
5. repeat steps 3 and 4 until content

## Gameplay
After selecting a character, the player attempts to move the character tile by tile up the screen to the water. Each touch of the water resets the character's position to the bottom of the screen and adds points to the score. Each collision with a bug subtracts one life and points from the score. Extra gem pickups appear at the beginning of the level. At a certain score amount an optional escape door opens, allowing the player to exit the level. If the character leaves the level or the player runs out of lives, the game ends and the final score is shown.

## History
This project was forked and modified from a Udacity project in order to complete the Object-Oriented JS course.
- project: Arcade Game (final project)
- course: Object-Oriented JavaScript
- instructor: Marcus Phillips
- platform: Udacity
- forked by: Botmasher (Joshua R) to complete the final project for Udacity OO JS

As an OO JS project, this game was expected to follow this [rubric](https://www.udacity.com/course/viewer/#!/c-nd001/l-2696458597/m-2687128535) and this [guide](https://docs.google.com/document/d/1v01aScPjSWCCWQLIpFqvg3-vXLH2e8_SZQKC8jNO0Dc/pub?embedded=true).

I returned to this game in early 2018 to update the art and interface, setting it apart somewhat from the original course project. The basic game rules are not changed from the intended goals of frontend-nanodegree-arcade-game, though extra features like scoring and exiting the level are added.

## Files and folders
This project is roughly divided into screens, scripts and assets. Index (start), game and gameover screens are built in HTML and styled with CSS. Assets include images displayed as in-game sprites and audio files. Scripts include the engine, the main app and the loading utilities.

## Sprites
Images are located within `/images`. All images are loaded in `Engine.js`. The world tiles are also arranged in the engine. The player character image is selected in `app.js` based on a parameter passed from the user selection made in `index.html`, where displayed character images are loaded separately in the HTML. The life hearts are displayed and updated in `game.html`. Because these locations are hardcoded in the four files above, changing all images requires changes to the URLs in all four.

The forked project initially included sprites provided by the Udacity course. Sprites were changed to my hand-drawn assets (affixed with `-sketch`) in January 2018.

## Collaborating
If you want to get involved in my fork of this project, feel free to download, fork or clone this project. After testing the game and looking through the code, you can start by opening issues about the documentation or code worth addressing in a PR.
