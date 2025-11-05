# React Tetris Dev

A modern, responsive Tetris game built with React, featuring smooth animations, touch controls, and a 3D visual theme option.

![Tetris Game](https://img.shields.io/badge/React-16.12.0-blue) ![Styled Components](https://img.shields.io/badge/Styled--Components-5.0.1-pink)

## Features

- **Responsive Design**: Automatically adapts to portrait and landscape orientations
- **Multiple Control Methods**:
  - Keyboard controls (arrow keys, spacebar)
  - Touch gestures for mobile devices
  - Click to rotate pieces
- **Visual Themes**: Toggle between classic 2D and modern 3D block styles
- **Progressive Difficulty**: Speed increases with each level
- **Score System**: 
  - Points awarded for clearing lines
  - Bonus multipliers for level and multiple lines cleared simultaneously
  - Track your score, level, and total lines cleared
- **Next Piece Preview**: See the upcoming Tetromino
- **Ghost Piece**: Visual hint showing where the current piece will land
- **Pause Functionality**: Automatically pauses when window loses focus

## Installation

### Prerequisites

- Node.js (version 16 or higher recommended)
- npm or yarn

### Setup

1. Clone the repository:
```bash
git clone https://github.com/yourusername/react-tetris.git
cd react-tetris
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

The game will open in your browser at `http://localhost:3000`

## Available Scripts

- `npm start` - Runs the app in development mode
- `npm run build` - Builds the app for production
- `npm test` - Launches the test runner
- `npm run deploy` - Deploys to GitHub Pages

## How to Play

### Keyboard Controls

- **Left Arrow** - Move piece left
- **Right Arrow** - Move piece right
- **Up Arrow** - Rotate piece clockwise
- **Down Arrow** - Soft drop (faster falling)
- **Spacebar** - Hard drop (instant placement)

### Touch Controls (Mobile)

- **Swipe Left/Right** - Move piece horizontally
- **Tap** - Rotate piece
- **Swipe Down** - Soft drop
- **Fast Swipe Down** - Hard drop

### Gameplay

1. Click "Start" to begin
2. Control falling Tetrominos to create complete horizontal lines
3. Clear lines to earn points and progress through levels
4. Game ends when pieces stack to the top of the board
5. Click "Restart" on the Game Over screen to play again

## Scoring System

- **Base Points**: 300 points per line cleared
- **Combo Bonus**: 40 × (lines² - 1) for clearing multiple lines at once
- **Level Bonus**: 100 × level² added to each clear

### Examples:
- 1 line: 300 + level bonus
- 2 lines: 600 + 40 + level bonus
- 3 lines: 900 + 320 + level bonus
- 4 lines (Tetris): 1200 + 600 + level bonus

## Technology Stack

- **React** (16.12.0) - UI framework
- **Styled Components** (5.0.1) - Styling solution
- **React Spring** (8.0.27) - Animation library
- **React Use Gesture** (7.0.5) - Touch gesture handling
- **Color** (3.1.2) - Color manipulation utilities

## Docker Support

Build and run the application using Docker:

```bash
docker build -t react-tetris .
docker run -p 3000:3000 react-tetris
```

## Project Structure

```
src/
├── components/
│   ├── Center/         # Centered container component
│   ├── Game/           # Main game logic and state management
│   ├── LoseGame/       # Game over screen
│   ├── Stage/          # Game board rendering
│   ├── StartPage/      # Start screen
│   ├── StatusRow/      # Score display component
│   └── Tetris/         # Root game component
├── hooks/
│   ├── useInterval.js  # Custom interval hook
│   └── useWindowDimensions.js  # Responsive sizing hook
├── utils/
│   └── Utils.js        # Helper functions
├── images/             # Game assets
└── styles.css          # Global styles
```

## Browser Compatibility

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the MIT License.

## Credits

Built with React and inspired by the classic Tetris game.

## Future Enhancements

- [ ] High score persistence
- [ ] Sound effects and background music
- [ ] Customizable themes
- [ ] Multiplayer support
- [ ] Touch gesture customization
- [ ] Achievement system

---

**Enjoy playing!** 🎮
