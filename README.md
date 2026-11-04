# word-master-design

This repository outlines the design of the pages and user interface for Wordmaster, as well as going over their functions.

All images were created using draw.io.

## Home
<img width="1102" height="852" alt="website-home drawio" src="https://github.com/user-attachments/assets/9ff3c6dd-d56d-4373-9a1a-02e1401d9868" />

The home page functions as more of a settings menu to start the game. On this page, different settings can be configured for making the game harder or easier. These settings will be carried over into the game. At the bottom of the page is a button for starting the game.
The navigation bar at the top of the page will remain consistent throughout the site, the current page will be highlighted by being italicized.

## Game
<img width="1102" height="852" alt="website-game drawio" src="https://github.com/user-attachments/assets/a8ead446-8b41-4198-be84-aa5099841205" />

The game page is the primary page for the site. The game can be played by typing words in and entering them to check if they are the correct word. The current guess is displayed at the top row of squares; letters filling in as the player types or removes characters.
The rows below the topmost row are for each guess. For every guess entered, it will appear in the next row that hasn't been filled in, certain letters are highlighted in yellow or green if their position is correct or not. If the player guesses the word, they win. If they run out of guesses, they lose.
At the start of the game a word is randomly pulled from a database with the selected difficulty options used for filtering. The game state is retained for each guess, and is only reset when a new game is started.
Two buttons at the top right corner are for starting over with the same settings, or going back to the home page.
In this example, the navigation bar is visible at the top. This is not final, though, as exiting the game page would cause a loss of game state.

## Stats
<img width="1102" height="852" alt="website-stats drawio" src="https://github.com/user-attachments/assets/ade0ea3b-69c8-4d98-b407-fd91f83900df" />

The stats page displays all the statistics for the player who is currently logged in. If you're not logged in, you will be redirected to the account page.
On this page, different stats like total games, win rate, and letter/word stats are displayed. Additionally, toggles for filtering stats for difficulty are present as well.
These stats are stored on a database and are updated with each game played. Users not logged in will not have their stats updated.

## Account
<img width="1102" height="852" alt="website-account drawio" src="https://github.com/user-attachments/assets/e00024f6-78f2-4b62-a49c-a76f46000a34" />

The account page lets a user log into their account or create a new one. Users can log into their account with the left panel, or create their account with the right panel.
Functionally, this page doesn't really need its own slot on the navigation bar. If not logged in, clicking account could take the user to the account page, and if logged in could take them to stats, where a button to sign out is present.
