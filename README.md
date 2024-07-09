## Quantum Checkers vs AI

This repository contains the code for a React-based game called "Quantum Checkers vs AI". This game is a twist on the classic Checkers game, incorporating elements of quantum mechanics.

**Game Features:**

- **Quantum Mechanics:** Each piece starts in a superposition state with a probability of being on the board. The probability is represented by the piece's opacity.
- **Quantum Operations:** Players can apply a rotation gate R(π/6) to their pieces after each move, increasing their probability of being on the board.
- **Capture and Measurement:** Captures involve measuring the quantum state of both the capturing piece and the target piece. If both are measured to be on the board, the capture succeeds. Otherwise, a global measurement occurs, removing pieces with low probability.
- **Kinging:** Pieces that reach the opposite end of the board become Kings and can move diagonally in any direction.
- **AI Opponent:** The game features a simple AI opponent that makes random moves, prioritizing captures.

**Installation:**

1. **Install Node.js:** Download and install the LTS (Long Term Support) version of Node.js from [https://nodejs.org/](https://nodejs.org/).
2. **Create a React Project:**
    - Open your command prompt or terminal.
    - Navigate to the directory where you want to create the project.
    - Run the following commands:
        ```bash
        npx create-react-app quantum-checkers
        cd quantum-checkers
        ```
3. **Install Tailwind CSS:**
    - In the project directory, run:
        ```bash
        npm install -D tailwindcss@latest postcss@latest autoprefixer@latest
        npx tailwindcss init -p
        ```
4. **Configure Tailwind CSS:**
    - Open the `tailwind.config.js` file in the project root and replace its content with:
        ```javascript
        module.exports = {
          content: [
            "./src/**/*.{js,jsx,ts,tsx}",
          ],
          theme: {
            extend: {},
          },
          plugins: [],
        }
        ```
5. **Add Tailwind Directives:**
    - Open `src/index.css` and add these lines at the top:
        ```css
        @tailwind base;
        @tailwind components;
        @tailwind utilities;
        ```
6. **Create QuantumCheckersGame Component:**
    - Create a new file named `QuantumCheckersGame.js` in the `src` folder.
    - Copy the entire code from the `QuantumCheckersGame` component in the provided `Quantum checkers vs AI - code.txt` file into this new file.
7. **Update App.js:**
    - Open `src/App.js` and replace its content with:
        ```javascript
        import React from 'react';
        import QuantumCheckersGame from './QuantumCheckersGame';

        function App() {
          return (
            <div className="App">
              <QuantumCheckersGame />
            </div>
          );
        }

        export default App;
        ```
8. **Start the Development Server:**
    - In the terminal, run the command:
        ```bash
        npm start
        ```
9. **View the Game:**
    - The development server should automatically open a new tab in Google Chrome.
    - If not, open Google Chrome and go to `http://localhost:3000`.

**You should now see the Quantum Checkers game running in your browser.**

**Game Manual:**

A detailed manual explaining the game rules and user interface is available in the `Quantum Checkers vs AI - Manual.pdf` file.

**Contribution:**

Feel free to contribute to this project! Submit pull requests for bug fixes, improvements, or new features.

**Enjoy playing Quantum Checkers!** 
