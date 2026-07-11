# Calculator

A simple, dark-themed calculator built with plain HTML, CSS, and JavaScript — no frameworks, no dependencies.

## 📁 File

`calculator.html` — everything (markup, styling, and logic) is in this single file.

## 🚀 Getting Started

No installation needed.

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```
2. Open `calculator.html` directly in your browser (double-click it, or right-click → "Open with").

## ✨ Features

- Standard operations: add, subtract, multiply, divide
- Percentage (`%`) and delete/clear (`DEL` / `AC`) functions
- Full keyboard support: number keys, `+ - * /`, `Enter` (equals), `Backspace` (delete), `Escape` (clear)
- Auto-formats large numbers with commas (e.g. `1,000`)
- Responsive, mobile-friendly layout

## 🛠️ Tech Stack

- **HTML5** — structure for the display and buttons
- **CSS3** — styling only (CSS variables for theming, CSS Grid for the button layout, gradients/transitions for polish)
- **Vanilla JavaScript (ES6+)** — all the logic, no libraries

## 🧠 How It Works

The logic is handled by a small `Calculator` class:

1. **State** — it keeps track of two numbers (`currOperand`, `prevOperand`) and the chosen operation (`+`, `−`, `×`, `÷`)
2. **Input** — clicking a number button appends it to the current number; clicking an operator saves the current number as "previous" and waits for the next number
3. **`compute()`** — runs the actual math when `=` (or Enter) is pressed
4. **Keyboard support** — the same functions are wired up to keydown events, so typing works just like clicking
5. **Display formatting** — a helper function adds commas to large numbers before showing them

No advanced concepts — just state, event listeners, and basic arithmetic.

## 📄 License

Free to use, modify, and share for personal or commercial projects.
