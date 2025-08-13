# Nixie Tube Clock

![Retro Neon Digital Clock](https://github.com/imtahirnaseer/Nixie-Tube-Light/blob/aebb5aed567cc5da51ff0e5124e8e3348d8a689b/nixie.png)

> **A retro-futuristic, photorealistic neon digital clock** — inspired by vintage Nixie tubes and powered by pure CSS magic.  
> Includes event display, interactive camera, engraved name, and festival listings.

---

## 📖 Table of Contents
- [Overview](#overview)
- [Live Demo](#live-demo)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Development Process](#development-process)
- [Detailed AI Prompt](#detailed-ai-prompt)
- [Installation & Usage](#installation--usage)
- [CSS Element Breakdown](#css-element-breakdown)
- [How Events Work](#how-events-work)
- [Customization](#customization)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)
- [License](#license)
- [Credits](#credits)

---

## Overview
This project recreates a **retro-futuristic neon digital clock** that combines:

- **Glowing segmented display** like old LED calculators/clocks.
- **Metallic tubular casing** inspired by Nixie tubes.
- **Right-side event panel** for Indian national & religious festivals.
- **Top rotating camera** that links to [my GitHub profile](https://github.com/imtahirnaseer).
- **Custom engraved name "Tahir"** with neon glow.
- **CSS-only visual effects**: metallic textures, neon bloom, film grain, flicker animations.

---

## 🔗 Live Demo 
Example: **[View Clock Live](https://imtahirnaseer.github.io/Nixie-Tube-Clock/)**

---

## ✨ Features
- **Core Clock** – Large digital time display (`12:34 AM` style) in neon orange/yellow.
- **Event Display** – Upcoming & past events with glowing LCD text.
- **Rotating Camera** – Visual scan effect + click link to GitHub.
- **Metallic & Neon Aesthetics** – CSS shadows, gradients, reflections.
- **Festival Coverage** – All major Indian festivals + scrolling events.
- **Photorealistic Effects** – Film grain overlay, bloom highlights, metallic depth.

---

## 🛠 Tech Stack
- **HTML5** – Semantic structure for the clock & panel.
- **CSS3** – Gradients, clip-paths, box shadows, filters, and custom fonts.
- **JavaScript (optional)** – For dynamic time update & event scrolling.
- **AI Image Tools** – (Optional) to generate static renderings.

---

## 📂 Project Structure
```

Nixie-Tube-Clock/
│
├── index.html         # Main HTML structure
├── nixie.png          # Sample generated image
├── README.md          # Project documentation
└── assets/            # Fonts, noise textures, icons

````

---

## 🏗 Development Process

### 1. **Concept & Inspiration**
- Chose a **Nixie tube style** because it blends vintage tech with neon aesthetics.
- Decided to **extend** it with an **event display panel** and **rotating camera**.

### 2. **Base Layout**
- Used **flexbox** to center the clock in the viewport.
- Set **dark gradient background** for mood.

### 3. **Outer Pipe Structure**
- Used `border-radius` + `clip-path` to shape the tube.
- Added **metallic gradients** for reflections.

### 4. **Inner Pipe & Glow**
- Multiple **box-shadows** to simulate depth and neon bloom.
- Color palette variables for **yellow/orange glow**.

### 5. **Time Display**
- Loaded **digital LCD fonts**.
- Added `text-shadow` layers for glow realism.

### 6. **Event Panel**
- Attached with a **connector bridge** to the main tube.
- Split into "Upcoming" and "Past" sections.
- Used fade & opacity for visual hierarchy.

### 7. **Rotating Camera**
- Circular lens with inner glow and scanning beam.
- Implied rotation using a **tilt angle** + motion blur.

### 8. **Engraving Name**
- Integrated **"Tahir"** on top metallic section with inset glow.

### 9. **Film Grain Overlay**
- SVG noise pattern at low opacity for retro realism.

### 10. **Final Touches**
- Flicker animations on neon parts.
- Depth shadows under the clock for floating effect.

---

>## 🎨 Detailed AI Prompt 
Instruction to AI Developer:
You are to create a fully functional, production-ready web application that replicates the described retro-futuristic Nixie Tube Clock exactly as specified. This must be a real working clock that updates time dynamically in real-time, includes an interactive rotating top camera element (clicking it opens https://github.com/imtahirnaseer), a right-side events/festivals panel with scrollable upcoming and past events, and engraved "Tahir" branding. The design must be built entirely in HTML, CSS, and vanilla JavaScript (no frameworks), with pixel-perfect adherence to the described visual design.

> Core Features:

Live Digital Clock:

Shows current time in HH:MM format with AM/PM indicator.

Time updates automatically every second.

Uses a segmented LCD/digital font for authenticity.

Neon glow effect around digits in warm orange/yellow shades.

Subtle flicker animation to simulate electric glow.

> Events Panel (Right Side):

Attached rectangular metallic panel aligned to main tube’s right side.

Divided into Upcoming Events (top) and Past Events (bottom).

Events array stored in JavaScript with dates; script automatically categorizes them based on current date.

Scroll or fade-in effect for multiple events.

Major Indian national and religious events included (Independence Day, Republic Day, Eid, Diwali, Christmas, Vaisakhi, etc.).

> Rotating Top Camera:

Circular metallic camera housing with glowing lens.

Slow continuous rotation animation (CSS transform: rotate() or JS-based).

Faint red scanning beam angled toward events panel.

Clickable — opens https://github.com/imtahirnaseer in a new tab.

> Name Engraving (“Tahir”):

Positioned on top metallic section.

Neon glow text effect with subtle metallic embossing.

> Aesthetics:

Retro-futuristic metallic casing with deep shadows and reflective highlights.

Neon orange (#ff8f0c), yellow (#fbd608), and red-orange (#b32801) glow palette.

Dark moody gradient background (#040909 to #312c2a).

Film grain overlay using CSS background or SVG noise texture.

Hexagonal glass tube pattern effect inside clock.

Glowing orange elliptical shadow pool beneath clock.

> Technical Requirements:

Entire project in one folder with index.html, style.css, and script.js.

Use requestAnimationFrame or setInterval for smooth time updates.

All colors, shadows, and gradients must match given hex values.

CSS variables for color palette for easy theme adjustment.

Responsive scaling based on viewport size (max 80vh height).

No external libraries except Google Fonts for LCD font.

Code must be clean, well-commented, and modular.

> Interactivity & Animations:

Camera rotation is infinite loop.

Clock digits glow intensity slightly varies (flicker simulation).

Event items fade in and out if more than 3 entries.

Hover effects on camera and engraved name.

># Output Format:
Provide the full HTML, CSS, and JS code in separate blocks, ensuring the project can be run locally by opening index.html in a browser.
Do not leave placeholders; include real sample events and working time display logic.
Ensure the design is visually identical to the described Nixie Tube Clock concept.

---

## 💻 Installation & Usage
```bash
# Clone the repo
git clone https://github.com/imtahirnaseer/Nixie-Tube-Clock.git
cd Nixie-Tube-Clock

# Open in browser
index.html
````

---

## 🔍 CSS Element Breakdown

| Element          | Purpose               | Key CSS Features                                 |
| ---------------- | --------------------- | ------------------------------------------------ |
| `.outer-pipe`    | Main tube casing      | `border-radius`, `clip-path`, metallic gradients |
| `.inner-pipe`    | Inner glowing section | Multi-layer `box-shadow` for depth               |
| `.display`       | Time digits           | LCD font, multi-color `text-shadow`              |
| `.event-panel`   | Festival display      | Flex layout, glow effects, divider               |
| `.camera`        | Rotating top camera   | Circular lens, gradient, scanning beam           |
| `.engraving`     | Name integration      | Inset shadows for metallic text                  |
| `.noise-overlay` | Film grain effect     | SVG pattern with opacity                         |

---

## 📅 How Events Work

* **Static Mode:** Hard-coded events in HTML.
* **Dynamic Mode:** Load from `events.json` and update panel automatically.
* Shows **2-3 upcoming** and **2-3 past** events at a time.
* Flicker effect for upcoming events for realism.

---

## 🛠 Customization

* Change **colors** via CSS variables:

```css
--_y1: #fae8a5; /* Yellow glow */
--_o1: #ff8f0c; /* Orange glow */
```

* Update `events.json` for different festivals.
* Change engraved name `"Tahir"` in HTML.

---

## 🚀 Future Improvements

* Real-time **time & date** updates.
* **Clickable events** with modal descriptions.
* **Theme switcher** for different neon colors.
* Full **JavaScript animation** for rotating camera.

---

## 🤝 Contributing

1. Fork the repo
2. Create a feature branch
3. Commit changes
4. Open a pull request

---

## 📜 License

MIT License — see [LICENSE](LICENSE).

---

## 🙏 Credits

* Design inspired by vintage electronics & Nixie tubes.
* Created by [Tahir Naseer](https://github.com/imtahirnaseer).
* Festivals list based on major Indian events.

cs. Created by [Tahir](https://github.com/imtahirnaseer).
