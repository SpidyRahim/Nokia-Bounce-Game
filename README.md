# 🔴 Nokia Bounce Game Recreation

A faithful recreation of the classic Nokia Bounce game built with vanilla HTML5, CSS, and JavaScript. No dependencies required!

![Bounce Game](https://img.shields.io/badge/Game-Bounce-red)
![HTML5](https://img.shields.io/badge/HTML5-Canvas-orange)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)
![License](https://img.shields.io/badge/License-MIT-green)

## 🎮 Play Now

Simply open `index.html` in your browser or [play the live demo here](#).

## 📸 Screenshots

```
<img width="1030" height="777" alt="image" src="https://github.com/user-attachments/assets/231b8d1d-a937-4560-af2f-db6e198684fb" />

```

## ✨ Features

- 🎯 **3 Progressive Levels** - Increasing difficulty with unique challenges
- 🔴 **Classic Bounce Physics** - Authentic bouncing ball mechanics
- 💛 **Ring Collection** - Gather all rings to unlock the exit
- 🔺 **Deadly Spikes** - Avoid or lose a life
- 🟢 **Inflate/Deflate System** - Change ball size to solve puzzles
- 🏁 **Checkpoint System** - Save progress within levels
- 📱 **Mobile Support** - Touch controls for mobile devices
- ✨ **Particle Effects** - Visual feedback for actions
- 🎨 **Retro Aesthetic** - Nokia-inspired visuals

## 🕹️ Controls

### Desktop

| Key | Action |
|-----|--------|
| `←` `→` or `A` `D` | Move left/right |
| `↑` or `W` or `Space` | Jump |
| `R` | Restart game |

### Mobile

Touch controls appear automatically on mobile devices:
- **Left Button** - Move left
- **Right Button** - Move right
- **Jump Button** - Jump

## 🎲 Game Elements

| Element | Description |
|---------|-------------|
| 🔴 Red Ball | Your character - bouncy and fun! |
| 💛 Rings | Collect all to unlock the exit door |
| 🔺 Spikes | Instant death - avoid at all costs |
| 🟢 Inflator (+) | Returns ball to normal size |
| 🔵 Deflator (-) | Shrinks ball to fit through tunnels |
| 🚩 Checkpoint | Activates respawn point |
| 🚪 Exit Door | Level complete (requires all rings) |

## 🚀 Getting Started

### Option 1: Direct Download

1. Download or clone this repository
   ```bash
   git clone https://github.com/yourusername/bounce-game.git
   ```

2. Open `index.html` in your web browser

3. Start playing!

### Option 2: Local Server

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (with http-server)
npx http-server

# Using PHP
php -S localhost:8000
```

Then navigate to `http://localhost:8000`

## 📁 Project Structure

```
bounce-game/
│
├── index.html      # Main game file (all-in-one)
├── README.md       # This file
└── LICENSE         # MIT License
```

## 🛠️ Technical Details

- **Pure Vanilla JS** - No frameworks or libraries
- **HTML5 Canvas** - Hardware-accelerated rendering
- **CSS3** - Modern styling with gradients and shadows
- **Responsive Design** - Works on all screen sizes
- **60 FPS** - Smooth gameplay using `requestAnimationFrame`

### Physics System

```javascript
// Core physics constants
const gravity = 0.6;
const friction = 0.8;
const bounce = 0.3;
const jumpForce = -15;
```

## 🎨 Customization

### Adding New Levels

Add a new level object to the `levels` array:

```javascript
{
    platforms: [
        { x: 0, y: 450, width: 400, height: 50 },
        // Add more platforms...
    ],
    rings: [
        { x: 200, y: 400 },
        // Add more rings...
    ],
    spikes: [
        { x: 300, y: 430, width: 40, height: 20 },
        // Add more spikes...
    ],
    inflators: [],
    deflators: [],
    checkpoints: [
        { x: 500, y: 260 }
    ],
    exit: { x: 900, y: 390 },
    startX: 100,
    startY: 400
}
```

### Modifying Ball Properties

```javascript
const ball = {
    radius: 20,        // Ball size
    speed: 5,          // Movement speed
    jumpForce: -15,    // Jump strength
    color: '#ff4444'   // Ball color
};
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. 🍴 Fork the repository
2. 🔧 Create a feature branch (`git checkout -b feature/amazing-feature`)
3. 💾 Commit your changes (`git commit -m 'Add amazing feature'`)
4. 📤 Push to the branch (`git push origin feature/amazing-feature`)
5. 🔃 Open a Pull Request

### Ideas for Contributions

- [ ] Add more levels
- [ ] Implement sound effects
- [ ] Add background music
- [ ] Create a level editor
- [ ] Add power-ups
- [ ] Implement a scoring system
- [ ] Add animations for the ball
- [ ] Create different ball skins

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2024 [Your Name]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:
...
```

## 🙏 Acknowledgments

- Original **Bounce** game by Nokia
- Inspired by the classic Nokia 3310 era games
- Thanks to all contributors and players!

## 📬 Contact

Your Name - [@yourtwitter](https://twitter.com/yourtwitter)

Project Link: [https://github.com/yourusername/bounce-game](https://github.com/yourusername/bounce-game)

---

<p align="center">
  Made with ❤️ and nostalgia
  <br>
  ⭐ Star this repo if you enjoyed playing!
</p>
