# AeroCalc — Modern Precision Calculator

A precision calculator web application designed with semantic HTML5, modern Tailwind CSS styling, and vanilla JavaScript. AeroCalc features real-time calculation previews, chained arithmetic with floating-point correction, a slide-out history tape with value recall, pure Web Audio tactile feedback, and full physical keyboard bindings.

---

## Features

- **Core Arithmetic Operations:** Addition ($+$), Subtraction ($-$), Multiplication ($\times$), and Division ($\div$).
- **Smart Display & Live Preview:**
  - Real-time anticipated result line that updates as you type the secondary operand.
  - Active operand display with automatic dynamic font scaling to prevent overflow.
  - Top expression line tracking equation state.
- **Floating-Point Precision:** Uses epsilon-safe rounding to prevent arithmetic quirks (such as $0.1 + 0.2 = 0.30000000000000004$).
- **Zero-Division Protection:** Displays graceful visual toast notifications without crashing application state.
- **Slide-Out History Tape:**
  - Keeps chronological track of past calculations with timestamps.
  - Click any prior log entry to recall its result directly into the active register.
  - Clear history with one click.
- **Physical Keyboard Support:** Full hotkey mapping with synchronized button-press animations.
- **Tactile Web Audio Synthesizer:** Real-time synthesized mechanical key clicks (no external MP3/audio files needed) with a mute toggle.
- **Glassmorphic UI & Color Themes:** Switch between Cyan, Amber, and Emerald themes.

---

## File Structure

```
├── index.html        # Standalone application (HTML, CSS, JS, audio synthesizer)
└── README.md         # Project documentation
```

---

## Getting Started

Because AeroCalc is completely self-contained, no build steps, Node packages, or server runtimes are necessary.

### 1. Direct Browser Launch
Clone or download this repository, then double-click `index.html` or open it from your terminal:

```bash
# On macOS
open index.html

# On Windows
start index.html

# On Linux
xdg-open index.html
```

### 2. Local HTTP Server (Optional)
```bash
# Using Node.js
npx serve .

# Or using Python 3
python3 -m http.server 8080
```

---

## Keyboard Shortcuts

| Key | Calculator Action |
| :--- | :--- |
| `0` – `9` | Input number digits |
| `.` | Insert decimal point |
| `+` | Addition |
| `-` | Subtraction |
| `*` | Multiplication ($\times$) |
| `/` | Division ($\div$) |
| `Enter` or `=` | Calculate result |
| `Backspace` | Delete last digit |
| `Escape` | Clear all (`AC`) |
| `%` | Percentage calculation |

---

## Tech Stack

- **HTML5:** Semantic document structure and accessibility attributes (`aria-live`, labels).
- **Tailwind CSS (CDN):** Responsive layouts, glassmorphism backdrop filters, and design system.
- **Vanilla JavaScript (ES6+):** State machine, expression calculation, and event handling.
- **Web Audio API:** Zero-dependency procedural synthesis for click feedback.
- **Lucide Icons:** Clean vector interface iconography.

---

## License

This project is open-source and free to use for personal or educational purposes.