# 🔐 Password Generator

A simple, dependency-free password generator built with vanilla HTML, CSS, and JavaScript. Customize length and character types, then generate and copy a secure password in one click.

![No frameworks](https://img.shields.io/badge/frameworks-none-informational)
![Vanilla JS](https://img.shields.io/badge/JavaScript-Vanilla-yellow)

## Preview

A dark-themed card UI with a live password display, a length slider, character-type checkboxes, and a copy-to-clipboard button.

## Features

- Adjustable password length (4–32 characters) via a range slider
- Toggle character types independently:
  - Uppercase letters (A–Z)
  - Lowercase letters (a–z)
  - Numbers (0–9)
  - Symbols (`!@#$%^&*()_-+=?`)
- One-click copy to clipboard, with a "Copied!" confirmation
- Guards against generating from an empty character pool
- No build step, no dependencies — just open the HTML file

## Tech Stack

- **HTML5** — structure
- **CSS3** — dark UI, no external frameworks
- **JavaScript (ES6)** — DOM manipulation, `Math.random()`, Clipboard API

## Getting Started

No installation required.

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/password-generator.git
   ```
2. Open `password-generator.html` in any browser.

That's it — no `npm install`, no server, no build tools.

## How It Works

1. Selected checkboxes determine which character sets are combined into a single pool.
2. `Math.random()` picks characters from that pool, one at a time, until the chosen length is reached.
3. The result is displayed and can be copied via the browser's Clipboard API.

## Project Structure

```
password-generator/
└── password-generator.html   # HTML, CSS, and JS all in one file
```

## Possible Improvements

- Password strength meter (weak / medium / strong)
- Option to exclude ambiguous characters (e.g. `0`, `O`, `l`, `1`)
- Save/generate multiple passwords at once
- Dark/light theme toggle

## License

This project is open source and available under the [MIT License](LICENSE).
