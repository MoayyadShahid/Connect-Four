# Connect Four Game - Developer Documentation

## Introduction
Welcome to my Connect Four project documentation. This web-based version of the classic Connect Four game is designed to be interactive, responsive, and user-friendly. The project encapsulates modern web development practices with a focus on modular architecture and efficient state management, ensuring a seamless gameplay experience across various devices.

## Project Structure
The project is structured into HTML, CSS, and JavaScript files, each serving distinct roles:

### HTML
- **index.html**: Serves as the entry point of the game. It organizes the game's layout including the main menu, game grid, and rule screen. It links to the CSS for styling and JavaScript for functionality.

### CSS
- **main.css**: Imports other CSS files and manages global styles.
- **fonts.css**, **general.css**, **components.css**, **layout.css**: These files collectively style the game, ensuring it is visually appealing and functionally responsive. They define fonts, general element styles, specific components, and the overall layout responsiveness.
  
### JavaScript
The JavaScript files utilize ES6 modules to separate concerns:
- **Game.js**: Acts as the game engine. It initializes the game, handles the logic for player turns, disc dropping, win checks, and manages game state transitions.
- **Grid.js**: Manages the game board data, calculating valid moves, storing disc positions, and checking for winning conditions.
- **View.js**: Manages all direct interactions with the DOM. It updates the game's visual components in response to state changes in `Game.js`.
- **Control.js**: Handles user inputs through event listeners, allowing players to interact with the game via mouse or keyboard.
- **Navigation.js**: Controls navigation between different parts of the game like menus and the game board itself, handling the transitions and state visibility.
- **helpers.js**: Provides utility functions to simplify DOM selection and iterative operations.

## How the Files Work Together
1. **HTML and CSS Integration**: The HTML file serves as the scaffold, defining the structure. CSS files are then applied to this structure, styling each component from the broad layout down to specific elements like buttons and the game grid.

2. **JavaScript Interaction**:
   - **Control Flow**: `Control.js` captures and manages user input, interacting directly with `Game.js` to affect the game state.
   - **Game Logic**: `Game.js` uses `Grid.js` to handle the logical representation of the game board and to determine game outcomes based on player actions.
   - **View Updates**: `View.js` listens to changes in game state from `Game.js` and updates the DOM accordingly, ensuring the player always has a current view of the game state.
   - **Navigation**: `Navigation.js` provides seamless transitions between different views like the main menu, game view, and rules screen, enhancing the user experience without reloading the page.

## Result
This Connect Four game is a full-featured web application that allows two players to compete in a classic game or against an AI opponent. It is designed to be visually engaging, easy to navigate, and accessible on multiple devices thanks to its responsive design. The modular JavaScript architecture allows for easy maintenance and scalability.

## Conclusion
Developed with best practices in web development, this project showcases my ability to architect and implement sophisticated web applications. It reflects a deep understanding of modern JavaScript, CSS, HTML, and responsive design principles. This documentation is aimed at providing fellow developers and recruiters with a clear view of the project's architecture and functionality, highlighting the careful consideration of design decisions and implementations.
