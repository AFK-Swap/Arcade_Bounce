# Arcade Bounce 🎮
**OpenGL-Based 2D Physics Simulation Game**

A complete arcade-style platformer game built from scratch using Python and OpenGL, featuring custom physics simulation, multi-level gameplay, and dynamic enemy AI.

## 📋 **Table of Contents**
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Installation](#installation)
- [Gameplay](#gameplay)
- [Controls](#controls)
- [Technical Implementation](#technical-implementation)
- [Project Structure](#project-structure)

## ✨ **Features**

### **Custom Graphics Engine**
- 🎨 **Pure OpenGL Rendering**: Built entirely with OpenGL for maximum performance
- 🖼️ **Procedural Graphics**: Custom drawing functions for all game elements
- ⚡ **Optimized Rendering**: Efficient vertex processing and pixel manipulation
- 🎭 **Dynamic Visual Effects**: Real-time color changes and animations

### **Advanced Physics System**
- 🌍 **Realistic Gravity**: Accurate gravitational acceleration and momentum
- 🦘 **Multi-Jump Mechanics**: Support for double-jump with physics constraints
- 💥 **Collision Detection**: Precise AABB collision detection for all objects
- 🏀 **Bounce Physics**: Realistic ball physics with velocity and acceleration

### **Multi-Level Gameplay**
- 🗺️ **Dynamic Maze System**: Procedurally changing level layouts
- 🚧 **Interactive Obstacles**: Moving platforms and destructible barriers
- 👾 **Intelligent Enemies**: AI-controlled enemies with patrol patterns
- 💎 **Treasure Collection**: Strategic collectibles affecting gameplay

### **Game Mechanics**
- ❤️ **Lives System**: 3-life system with game over functionality
- ⏸️ **Pause & Resume**: Full game state management
- 🔄 **Restart Functionality**: Quick game reset and replay
- 🎯 **Scoring System**: Point tracking and achievement rewards

### **Interactive Elements**
- 🎨 **Customizable Ball**: Color selection system with randomization
- 🔫 **Laser Obstacles**: Moving laser barriers with timing challenges
- 🏆 **Treasure Hunt**: Collectible items that pause laser systems
- 📊 **Real-time Stats**: Live display of lives, level, and progress

## 🛠️ **Technology Stack**

### **Core Technologies**
- **Python 3.x** - Main programming language
- **OpenGL** - Graphics rendering and 3D acceleration
- **PyOpenGL 3.1.6** - Python bindings for OpenGL
- **PyOpenGL-accelerate 3.1.6** - Performance optimizations

### **Standard Libraries**
- **Math** - Mathematical calculations for physics
- **Time** - Game timing and animation control
- **Random** - Procedural generation and randomization

### **Graphics Pipeline**
- **Custom Rendering Engine** - Built from scratch OpenGL implementation
- **Vertex Processing** - Manual vertex manipulation and transformation
- **Pixel-Perfect Collision** - Custom collision detection algorithms
- **Animation System** - Frame-based animation with smooth interpolation

## 🚀 **Installation**

### **Prerequisites**
- Python 3.6 or higher
- OpenGL support (usually included with graphics drivers)
- pip package manager

### **Quick Setup**
```bash
# Clone the repository
git clone https://github.com/AFK-Swap/Arcade_Bounce.git
cd Arcade_Bounce

# Install dependencies
pip install -r requirements.txt

# Alternative manual installation
pip install PyOpenGL==3.1.6 PyOpenGL-accelerate==3.1.6

# Run the game
python main.py
```

### **Requirements File**
```txt
PyOpenGL==3.1.6
PyOpenGL-accelerate==3.1.6
```

## 🎮 **Gameplay**

### **Objective**
Navigate through increasingly challenging levels, avoid enemies and laser obstacles, collect treasures, and reach the exit portal while managing your limited lives.

### **Game Flow**
1. **Menu Screen**: Choose ball color and start game
2. **Level 1**: Navigate basic obstacles and enemies
3. **Level 2**: Advanced maze with moving platforms
4. **Level 3**: Complex multi-phase challenges
5. **Victory**: Complete all levels with remaining lives

### **Scoring System**
- 🎯 **Survival**: Points for staying alive
- 💎 **Treasures**: Bonus points for collecting items
- ⚡ **Speed**: Time-based scoring multipliers
- 🏆 **Perfect**: Extra points for completing without deaths

## 🕹️ **Controls**

### **Movement**
- **A** / **←** - Move left
- **D** / **→** - Move right
- **Spacebar** - Jump (press twice for double-jump)

### **Game Management**
- **Mouse Click** - Menu interactions and game controls
- **Pause Button** - Pause/resume gameplay
- **Restart Button** - Reset current level
- **Exit Button** - Quit game

### **Menu Controls**
- **Color Arrows** - Change ball color
- **Next Button** - Start game
- **Exit Button** - Close application

## 💻 **Technical Implementation**

### **Custom OpenGL Engine**
```python
# Core rendering system
def drawLine(x1, y1, x2, y2, color_diff):
    # Bresenham's line algorithm implementation
    # Optimized pixel-by-pixel rendering
    
def midPointCircle(x, y, rad, r, g, b):
    # Midpoint circle algorithm
    # Efficient circle rendering without trigonometry
    
def drawCircle(xc, yc, r, color_diff):
    # Filled circle using triangle fan
    # Smooth circular objects
```

### **Physics Engine**
```python
# Gravity and jumping mechanics
def animate_ball():
    # Real-time physics calculation
    # Velocity, acceleration, and collision handling
    
def checkObstacleCollision(new_x, new_y):
    # AABB collision detection
    # Precise boundary checking
```

### **Game State Management**
```python
# Multi-level progression system
def display():
    # Render different game states
    # Menu, gameplay, game over screens
    
def mouseListener(button, state, x, y):
    # Input handling and game control
    # Menu navigation and game interactions
```

### **AI and Animations**
- **Enemy AI**: Predictable patrol patterns with boundary detection
- **Laser Systems**: Timed obstacle movement with collision detection
- **Treasure Effects**: Dynamic game state changes upon collection
- **Animation Loops**: Smooth enemy movement and visual effects

## 🏗️ **Project Structure**

```
Arcade_Bounce/
├── main.py                 # Main game file with complete implementation
├── requirements.txt        # Python dependencies
├── README.md              # This documentation
└── assets/                # Game assets (if any)
    ├── screenshots/       # Game screenshots
    └── docs/             # Additional documentation
```

### **Code Organization**
```python
# Main game components
- Game initialization and window setup
- Drawing and rendering functions
- Physics and collision detection
- Input handling and controls
- Game state management
- Enemy AI and animations
- Sound and visual effects
```

## 🎯 **Game Features Deep Dive**

### **Multi-Level Design**
- **Level 1**: Introduction with basic obstacles
- **Level 2**: Moving enemies and advanced platforms
- **Level 3**: Complex maze with multiple challenges
- **Phase System**: Dynamic level progression

### **Physics Accuracy**
- **Realistic Gravity**: 9.8 m/s² equivalent acceleration
- **Momentum Conservation**: Proper velocity calculations
- **Collision Response**: Accurate bounce and stop mechanics
- **Jump Mechanics**: Variable jump height based on input

### **Visual Effects**
- **Particle Systems**: Trail effects and explosion animations
- **Color Cycling**: Dynamic color changes and effects
- **Smooth Animations**: Interpolated movement and transitions
- **Visual Feedback**: Clear indicators for all interactions

## 🧪 **Testing & Debugging**

### **Performance Testing**
- ✅ 60+ FPS on modern hardware
- ✅ Memory usage optimization
- ✅ OpenGL context management
- ✅ Input responsiveness testing

### **Gameplay Testing**
- ✅ All collision scenarios
- ✅ Physics edge cases
- ✅ Level progression logic
- ✅ Game state persistence

## 🔧 **Development Notes**

### **OpenGL Implementation**
- Custom graphics pipeline built from scratch
- No external game engines or frameworks
- Direct OpenGL calls for maximum control
- Optimized for educational purposes and performance

### **Learning Outcomes**
- Computer graphics programming fundamentals
- Physics simulation and mathematical modeling
- Game loop architecture and timing
- Event-driven programming patterns
- Real-time system design

## 🤝 **Contributing**

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/NewFeature`)
3. Commit your changes (`git commit -m 'Add NewFeature'`)
4. Push to the branch (`git push origin feature/NewFeature`)
5. Open a Pull Request


## 👨‍💻 **Author**

**Fahmidur Iqbal Swapnil**
- GitHub: [@AFK-Swap](https://github.com/AFK-Swap)
- Email: fahmidur.i.swapnil@gmail.com
- University: BRAC University

## 🙏 **Acknowledgments**

- OpenGL community and documentation
- Computer graphics programming resources
- BRAC University CSE Department
- Game development learning communities

---

*A showcase of custom game engine development and computer graphics programming* 🚀

