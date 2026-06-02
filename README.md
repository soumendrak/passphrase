<div align="center">

# Passphrase

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen?style=flat-square)](https://soumendrak.github.io/passphrase/)
[![MIT License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)](LICENSE)
[![HTML5](https://img.shields.io/badge/HTML5-%23E34F26?style=flat-square&logo=html5&logoColor=white)](https://html.spec.whatwg.org/)
[![Zero Dependencies](https://img.shields.io/badge/dependencies-0-success?style=flat-square)](https://www.w3.org/TR/html52/)

<!-- Inline SVG logo -->
<svg width="140" height="140" viewBox="0 0 140 140" xmlns="http://www.w3.org/2000/svg">
<rect width="140" height="140" rx="24" fill="#0a0a14"/>
  <text x="70" y="42" text-anchor="middle" font-family="monospace" font-size="8" fill="#f0ece4">correct</text>
  <text x="70" y="55" text-anchor="middle" font-family="monospace" font-size="8" fill="#f0ece4">horse</text>
  <text x="70" y="68" text-anchor="middle" font-family="monospace" font-size="8" fill="#f0ece4">battery</text>
  <text x="70" y="81" text-anchor="middle" font-family="monospace" font-size="8" fill="#f0ece4">staple</text>
  <rect x="30" y="100" width="80" height="4" rx="2" fill="#1a1a2e"/>
  <rect x="30" y="100" width="56" height="4" rx="2" fill="#ff6b35"/>
  <text x="70" y="118" text-anchor="middle" font-family="sans-serif" font-size="7" fill="#8a8a9a">52 bits of entropy</text>
</svg>

**Diceware-style passphrase generator — strong, memorable, and configurable.**

**Live:** [https://soumendrak.github.io/passphrase/](https://soumendrak.github.io/passphrase/)

</div>

---

## Features

- Built-in word list of 2,300+ common English words
- Slider: 3-8 words
- Toggle: capitalize, +digit, +special character
- Separator choice: space, hyphen, dot, underscore
- Entropy indicator with visual rating bar (bits of security)
- Auto-copy to clipboard
- 'Another' button for quick re-rolls
- Dark theme with orange accent (#ff6b35)

## How It Works

Words are selected randomly using `crypto.getRandomValues()` for cryptographically secure randomness. Entropy is calculated as `log2(wordListSize^wordCount) + log2(digitChars) + log2(specialChars)` for enabled options. The rating bar compares entropy against a threshold: green (>80 bits), amber (60-80), or red (<60).

## Usage

1. Open `https://soumendrak.github.io/passphrase/` in any browser.
2. No build step, no installation, no server required.
3. Deploy anywhere — GitHub Pages, Netlify, or any static host.

```bash
git clone https://github.com/soumendrak/passphrase.git
# Open index.html directly
```

## License

Licensed under the [MIT License](LICENSE).

---

<p align="center"><sub>Built with ❤️ and zero dependencies</sub></p>
