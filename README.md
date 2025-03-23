# Tic-Tac-Toe
HTML Structure (index.html)
The HTML file sets up the basic structure of the Tic-Tac-Toe game. It includes the following elements:

DOCTYPE and HTML Tag:

Declares the document type and starts the HTML document.

Head Section:
Contains meta tags for character set and viewport settings.
Includes the title of the page.
Links to the external CSS file (style.css) for styling.

Body Section:
Contains a heading (<h1>) for the game title.
A container (<div class="container">) that holds the game board and the reset button.
Inside the container, there is a game board (<div class="game">) with 9 boxes (<div class="box">) representing the Tic-Tac-Toe grid.
A reset button (<button id="reset-btn">Reset</button>) to reset the game.
A message container (<div class="msg-container hide">) that displays the game result (win or draw) and a new game button.
Inside the message container, there is a message display (<div id="msg"></div>) and a new game button (<button id="new-btn">New Game</button>).
A script tag to include the external JavaScript file (app.js) for game logic.

CSS Styling (style.css)
The CSS file styles the game elements to make them visually appealing and functional:

Global Styles:
Resets margin and padding for all elements to zero.

Body Styles:
Sets the background color, text alignment, and layout properties to center the content vertically and horizontally.

Heading Styles:
Styles the game title with margin, font size, and color.

Container Styles:
Sets the height and layout properties to center the game board and reset button.

Game Board Styles:
Sets the dimensions, layout properties, and gap between the boxes.

Box Styles:
Styles each box with dimensions, border radius, shadow, font size, background color, and layout properties to center the text inside.

Box Class Styles:
Defines specific colors for "X" and "0" using .box.x and .box.o classes.

Button Styles:
Styles the reset and new game buttons with padding, font size, background color, text color, border radius, and margin.

Message Container Styles:
Styles the message container to cover the entire screen with a semi-transparent background and center the content.

Hide Class:
Defines a class to hide elements using display: none.

JavaScript Logic (app.js)
The JavaScript file contains the game logic to handle user interactions and game state:

Variable Declarations:
Selects DOM elements for the boxes, reset button, new game button, message container, and message display.
Initializes variables to track the current turn (turn0), move count (count), and winning patterns (winPatterns).

Reset Game Function:
Resets the game state, enables all boxes, and hides the message container.

Game Draw Function:
Displays a draw message, shows the message container, and disables all boxes.

Disable Boxes Function:
Disables all boxes to prevent further clicks.

Enable Boxes Function:
Enables all boxes, clears their content, and removes any applied classes.

Show Winner Function:
Displays the winner message, shows the message container, and disables all boxes.

Check Winner Function:
Checks if there is a winning pattern by comparing the values of the boxes. If a winner is found, it calls the showWinner function.

Event Listeners for Boxes:
Adds click event listeners to each box. When a box is clicked, it updates the box content and class based on the current turn, disables the box, increments the move count, and checks for a winner or draw.

Event Listeners for Buttons:
Adds click event listeners to the reset and new game buttons to reset the game when clicked.

This code sets up a functional Tic-Tac-Toe game where players can click on boxes to place "X" or "0", and the game checks for a winner or draw after each move. The reset and new game buttons allow players to start a new game.
