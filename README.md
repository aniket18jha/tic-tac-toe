# React Tic-Tac-Toe Project

This project is a React-based implementation of the classic Tic-Tac-Toe game. Below, you'll find the steps to start the project, the tech stack used, and the React concepts applied in the project.

---

## How to Start the Project

1. **Clone the Repository**  
   Clone the project repository to your local machine:
   ````bash
  # git clone <repository-url>
  # cd 07-tic-tac-toe-starting-project
  # npm install
  # npm run dev
  # Collecting workspace information```markdown
   ````

# React Tic-Tac-Toe Project

This project is a React-based implementation of the classic Tic-Tac-Toe game. Below, you'll find the steps to start the project, the tech stack used, and the React concepts applied in the project.

---

## How to Start the Project

1. **Clone the Repository**  
   Clone the project repository to your local machine:

  
   git clone <repository-url>
   cd 07-tic-tac-toe-starting-project
  

2. **Install Dependencies**  
   Install the required dependencies using npm:

   ```bash
   npm install
   ```

3. **Start the Development Server**  
   Run the development server using Vite:

   ```bash
   npm run dev
   ```

4. **Access the Application**  
   Open your browser and navigate to the URL provided by Vite (usually `http://localhost:5173`).

---

## Tech Stack

- **React**: A JavaScript library for building user interfaces.
- **Vite**: A fast build tool and development server for modern web projects.
- **JavaScript (ES6+)**: Modern JavaScript features like arrow functions, destructuring, and template literals.
- **CSS**: Custom styling for the game UI.
- **Node.js**: For managing dependencies and running the development server.

---

## React Concepts Used

### 1. **Functional Components**

- The project uses functional components to define the UI and logic for different parts of the application.
- Examples:
  - [`App`](src/App.jsx)
  - [`Player`](src/components/Player.jsx)
  - [`GameBoard`](src/components/GameBoard.jsx)
  - [`Log`](src/components/Log.jsx)
  - [`GameOver`](src/components/GameOver.jsx)

### 2. **State Management with `useState`**

- The `useState` hook is used to manage the state of the application, such as:
  - Player names (`players` state in [`App`](src/App.jsx)).
  - Game turns (`gameTurns` state in [`App`](src/App.jsx)).
  - Editing player names (`isEditing` state in [`Player`](src/components/Player.jsx)).

### 3. **Props**

- Props are used to pass data and event handlers between components.
- Examples:
  - Passing `onSelectSquare` and `board` props to [`GameBoard`](src/components/GameBoard.jsx).
  - Passing `winner` and `onRestart` props to [`GameOver`](src/components/GameOver.jsx).

### 4. **Derived State**

- The active player is derived from the `gameTurns` state using the `deriveActivePlayer` function in [`App`](src/App.jsx).

### 5. **Conditional Rendering**

- Conditional rendering is used to display different UI elements based on the game state.
- Examples:
  - Showing the `GameOver` component when the game ends.
  - Displaying "Edit" or "Save" buttons in the [`Player`](src/components/Player.jsx) component based on the `isEditing` state.

### 6. **Event Handling**

- Event handlers are used to handle user interactions, such as:
  - Clicking a square on the game board (`handleSelectSquare` in [`App`](src/App.jsx)).
  - Editing player names (`handleEditClick` in [`Player`](src/components/Player.jsx)).

### 7. **Lists and Keys**

- The game board and log are rendered as lists using the `map` function.
- Unique keys are assigned to list items to optimize rendering.

### 8. **CSS Styling**

- The project uses a custom CSS file ([`index.css`](src/index.css)) for styling.
- Animations and responsive design are included for a better user experience.

---

## Concepts Demonstrated in the Game

1. **Dynamic Player Names**  
   Players can edit their names dynamically, demonstrating the use of state and controlled components.

2. **Game State Management**  
   The game board and turns are managed using state, and the UI updates dynamically based on the state.

3. **Win and Draw Detection**  
   The game logic includes detecting winning combinations and handling draws.

4. **Restart Functionality**  
   The game can be restarted at any time, resetting the state to its initial values.

5. **Component Reusability**  
   Components like `Player` and `GameBoard` are reusable and modular.

---

## Future Improvements

- Add single-player mode with AI.
- Enhance the UI with animations and sound effects.
- Add a feature to save and load game states.
- Improve accessibility for better usability.

---

## License

This project is licensed under the MIT License.

```

```
