# QUADRA - Tetris Game

**Live Demo:** https://dannellbayer.com/Tetris/

## Project Overview

QUADRA is a browser-based Tetris clone built as my first JavaScript school project. The game features classic Tetris gameplay where players stack falling tetrominoes to form complete rows, which then disappear and award points.

**Playable on both desktop and mobile devices.**

## Controls

### Desktop (Keyboard)
| Key | Action |
|-----|--------|
| ← | Move left |
| → | Move right |
| ↑ | Rotate piece |
| ↓ | Move down |

### Mobile (Touch)
On-screen buttons allow full gameplay control using touch events.

## Technical Implementation

### Core Features
- **5 Tetromino Types**: L, Z, T, O, and I pieces, each with unique rotation states
- **Rotation System**: Each piece rotates through 4 positions (except O which stays the same)
- **Collision Detection**: Prevents pieces from overlapping walls, floor, or other placed pieces
- **Line Clearing**: Complete rows disappear, pieces above fall down, score increases
- **Next Piece Preview**: Shows the upcoming tetromino in a mini-grid
- **Game Over Detection**: Triggers when a new piece cannot spawn without overlapping
- **Start/Pause Toggle**: Single button controls the game state

### Technologies Used
- **JavaScript (Vanilla)**: Game logic, DOM manipulation, event handling
- **CSS3**: Flexbox layout, box-shadow effects, transitions, custom styling
- **HTML5**: Semantic structure with game grids built from div elements
- **Google Fonts**: Bungee Shade (title), Rubik (UI text)
- **Font Awesome**: Icon library for mobile control buttons
- **External APIs**: Google Fonts CDN, Font Awesome CDN

### Skills Demonstrated
- Array manipulation and iteration for grid management
- Modular function design (draw, undraw, freeze, move, rotate)
- State management (timer IDs, current position, rotation, score)
- Event-driven programming (keyboard and pointer events)
- CSS positioning and box-sizing for consistent layouts
- Responsive design with viewport meta tag and touch controls

## File Structure
```
Tetris/
├── index.html          # Game markup and structure
├── js/
│   └── app.js          # All game logic
├── css/
│   ├── style.css       # Main styles
│   └── BrowserReset.css # CSS reset
├── images/
│   └── tetris.png      # Background image
├── README.md
└── SPEC.md
```

## Design Choices

- **Color Palette**: Teal (#30abbb) primary, purple (#302472) accents, soft blue (#8cafcc) grids
- **Typography**: Bungee Shade for the logo gives a block-built aesthetic matching the game theme
- **Shadows**: Custom box-shadows create depth and a polished feel
- **Mobile-First**: Touch controls with pointer events ensure cross-device compatibility