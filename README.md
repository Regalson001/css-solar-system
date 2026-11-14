# ☀️ CSS Solar System — Interactive Orbital Mechanics Engine

<p align="center">
  <strong>An animated solar system experience engineered entirely with HTML5 and CSS3.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-Structure-orange?style=for-the-badge&logo=html5" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-Animations-blue?style=for-the-badge&logo=css3" alt="CSS3">
  <img src="https://img.shields.io/badge/JavaScript-Not%20Required-lightgrey?style=for-the-badge" alt="No JavaScript">
  <img src="https://img.shields.io/badge/Responsive-Design-success?style=for-the-badge" alt="Responsive design">
</p>

---

## 🚀 Project Overview

**CSS Solar System** is a creative front-end engineering project that recreates an animated solar system using only HTML and CSS.

The experience features a central Sun, eight orbiting planets, nested moon animations, planetary information tooltips, glowing orbital paths, and a dark space-inspired interface.

Each planet follows its own continuous CSS animation. Nested rotational transforms allow planetary elements to counter-rotate while their orbital containers rotate. CSS hover and focus states provide interactive behaviour without JavaScript.

The project demonstrates how CSS can be used to build complex motion systems, layered visual interfaces, and interactive experiences.

## 🌐 Live Demo

**GitHub Repository:**

https://github.com/Regalson001/css-solar-system

**Live Website:**

https://regalson001.github.io/css-solar-system/

*The live URL becomes available after GitHub Pages deployment.*

## ✨ Features

### 1. Animated Solar System
- Central glowing Sun.
- Eight animated planetary orbits.
- Independent orbital durations.
- Continuous rotational animations.
- Layered orbital paths.
- Responsive solar system presentation.

### 2. Eight Planetary Representations
- Mercury
- Venus
- Earth
- Mars
- Jupiter
- Saturn
- Uranus
- Neptune

Each planet has its own visual appearance, colour scheme, orbital speed, and information tooltip.

### 3. Nested Orbital Mechanics
- Independent planet rotation.
- Counter-rotating planet elements.
- Nested moon orbit containers.
- Separate moon animation speeds.
- Continuous CSS rotation.

### 4. Interactive Planet Information
- Glassmorphic information tooltips.
- Hover-triggered visibility.
- Keyboard focus support.
- Planet facts and orbital periods.
- CSS-based animation pause states.

### 5. Planetary Information Dashboard
- Eight planet information cards.
- Planetary orbital period displays.
- Visual planet identifiers.
- Hover transitions.

### 6. Space-Inspired Interface
- Dark astronomical background.
- Animated stars.
- Glowing Sun and planets.
- Neon orbital rings.
- Glassmorphic information panels.

### 7. Responsive Design
- Desktop, tablet, and mobile layouts.
- CSS Grid and Flexbox.
- Responsive scaling of the solar system.
- Mobile-friendly information cards.
- Reduced-motion accessibility support.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| HTML5 | Semantic page structure |
| CSS3 | Visual design and styling |
| CSS Animations | Continuous orbital movement |
| CSS Transforms | Planet and moon rotation |
| CSS `:has()` | Parent-state interaction |
| CSS `:hover` | Interactive tooltips |
| CSS `:focus-visible` | Keyboard interaction |
| CSS Variables | Reusable design system |
| CSS Gradients | Planet surfaces and lighting |
| CSS Grid | Planet information dashboard |
| CSS Media Queries | Responsive layouts |
| Glassmorphism | Tooltip presentation |

**No JavaScript, frameworks, animation libraries, or build tools are required.**

## 🧠 Advanced CSS Techniques Demonstrated

### 1. Nested Rotational Transforms

The solar system uses nested elements to create independent orbital motion.

```css
.orbit {
  animation: orbit-spin linear infinite;
}

.planet {
  animation: counter-spin linear infinite;
}
```

The orbital container rotates in one direction while its planet counter-rotates to maintain a consistent visual orientation.

### 2. CSS Keyframe Animations

Continuous rotation is implemented using:

```css
@keyframes orbit-spin {
  from {
    transform: translate(-50%, -50%) rotate(0deg);
  }

  to {
    transform: translate(-50%, -50%) rotate(360deg);
  }
}
```

Different durations produce different visual orbital speeds.

### 3. Independent Moon Orbits

Moons are placed inside their parent planet elements and receive their own animation:

```css
.moon-orbit {
  animation: orbit-spin 3s linear infinite;
}
```

This demonstrates how nested CSS animations can create multiple layers of motion.

### 4. CSS `:has()` Interaction

The project uses the relational selector to pause an orbit when its planet is hovered or focused.

```css
.orbit:has(.planet:hover),
.orbit:has(.planet:focus-visible) {
  animation-play-state: paused;
}
```

### 5. Glassmorphism

Tooltips use transparency, blur, borders, and shadows.

```css
.tooltip {
  background: rgba(15, 25, 49, 0.88);
  backdrop-filter: blur(15px);
  border: 1px solid rgba(101, 232, 255, 0.4);
  border-radius: 10px;
}
```

### 6. CSS Custom Properties

Reusable colours and design tokens are stored in `:root`.

```css
:root {
  --space: #050713;
  --cyan: #65e8ff;
  --purple: #a98bff;
  --gold: #ffd36e;
}
```

### 7. Responsive Layout Engineering

Media queries control the solar system scale and information dashboard across different screen sizes.

### 8. Accessibility

The implementation includes:
- Keyboard-focusable planets.
- Visible focus outlines.
- Descriptive accessible labels.
- Reduced-motion preferences.
- Focus-triggered information tooltips.

## 📂 Project Structure

```text
css-solar-system/
│
├── index.html
│   └── Main solar system structure
│
├── styles.css
│   └── Planet styling, orbital mechanics and animations
│
├── README.md
│   └── Project documentation
│
├── LICENSE
│   └── MIT License
│
└── .gitignore
    └── Git exclusion rules
```

## ⚙️ Getting Started

### Prerequisites

- Visual Studio Code or another code editor.
- A modern web browser.
- Git installed on your computer.
- A GitHub account.

### 1. Clone the Repository

```bash
git clone https://github.com/Regalson001/css-solar-system.git
```

### 2. Navigate to the Project

```bash
cd css-solar-system
```

### 3. Open in Visual Studio Code

```bash
code .
```

### 4. Run the Project

Open `index.html` in your browser or use the Live Server extension in Visual Studio Code.

The planetary animations start automatically when the page loads.

## 🎯 Learning Objectives

This project provides practical experience with:

- Advanced CSS animation techniques.
- Nested rotational transformations.
- CSS animation timing and duration.
- Orbital-style motion systems.
- Counter-rotation techniques.
- Independent child animations.
- CSS relational selectors.
- Glassmorphic interface design.
- Keyboard-accessible interactions.
- Responsive front-end development.
- CSS-only interactive experiences.

## ⚠️ Scientific and Technical Scope

This is a visual CSS demonstration inspired by the solar system, not a scientifically accurate orbital mechanics engine.

- Orbital speeds are illustrative and not proportional to real astronomical periods.
- Orbit paths are circular rather than physically calculated elliptical trajectories.
- Planet sizes and distances are not to scale.
- The Sun and planets are CSS-rendered visual representations.
- Moon orbits are simplified visual animations.
- No astronomical data service or physics engine is connected.
- Hover and focus interactions are CSS-driven.

## 🔮 Future Improvements

Potential enhancements include:

- More moons for Earth, Jupiter, and Saturn.
- Additional planetary satellites.
- Elliptical orbit paths.
- Tilted orbital planes.
- Planet surface textures.
- A CSS-controlled orbital speed selector.
- A separate planet exploration interface.
- More detailed planetary information.
- Optional JavaScript-powered simulation controls.
- Improved small-screen planetary labels.

## 📸 Project Preview

Capture a screenshot of the completed solar system and save it in an `assets` folder.

```text
css-solar-system/
│
└── assets/
    └── solar-system-preview.png
```

Then add this to the README:

```markdown
![CSS Solar System Preview](./assets/solar-system-preview.png)
```

## 🌍 Deployment with GitHub Pages

1. Open the GitHub repository.
2. Navigate to **Settings**.
3. Select **Pages**.
4. Choose **Deploy from a branch**.
5. Select `main`.
6. Select `/(root)`.
7. Click **Save**.

Your project will be published at:

https://regalson001.github.io/css-solar-system/

## 👨‍💻 Author

**Stephen Oyugi**

Front-End Developer | AI Automation Practitioner | Machine Learning Practitioner

📍 Nairobi, Kenya

- **GitHub:** https://github.com/Regalson001
- **LinkedIn:** https://linkedin.com/in/stephenoyugi001
- **Email:** stephennyarangi03@gmail.com

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

<p align="center">
  <strong>Designed and developed by Stephen Oyugi.</strong>
</p>

<p align="center">
  Exploring motion, engineering interfaces, and building with CSS.
</p>
