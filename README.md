<div align="center">

# ⚡ ReactTailwind.com

**One script. Zero config. Start building in seconds.**

[![React](https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=white)](https://react.dev)
[![Vite](https://img.shields.io/badge/Vite-6-646CFF?style=flat-square&logo=vite&logoColor=white)](https://vitejs.dev)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-v4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)](https://tailwindcss.com)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)

[Website](https://reactvitetailwind.com) · [Report Bug](https://github.com/alejandrodlrocha/reactvitetailwind/issues) · [Request Feature](https://github.com/alejandrodlrocha/reactvitetailwind/issues)

---

</div>

## 🤔 Why?

Setting up React + Vite + Tailwind manually means:

- Creating the Vite project
- Installing Tailwind + PostCSS
- Creating `postcss.config.js`
- Configuring `index.css`
- Cleaning up boilerplate files
- Hoping you didn't miss a step

**This script does all of that in one command.**

## 🚀 Quick Start

### macOS / Linux

```bash
curl -fsSL https://reactvitetailwind.com/setup.sh | bash
```

Or download and run manually:

```bash
# Download
curl -O https://reactvitetailwind.com/setup.sh

# Make executable
chmod +x setup.sh

# Run
./setup.sh
```

### Windows (PowerShell)

```powershell
irm https://reactvitetailwind.com/setup.ps1 | iex
```

Or download and run manually:

```powershell
# Download
Invoke-WebRequest -Uri https://reactvitetailwind.com/setup.ps1 -OutFile setup.ps1

# Run
.\setup.ps1
```

## ✨ What You Get

```
my-app/
├── node_modules/
├── public/
├── src/
│   ├── App.jsx          # Animated demo component
│   ├── index.css         # Tailwind imports + custom animations
│   └── main.jsx
├── index.html
├── package.json
├── postcss.config.js     # Tailwind v4 PostCSS setup
└── vite.config.js        # Vite config (auto-open disabled)
```

### The Demo Component

The generated `App.jsx` includes:

- 🌊 Animated gradient blobs
- 💎 Glassmorphism card effect
- ✨ Interactive counter with state
- 🎨 Gradient text
- 🔘 Hover animations on buttons
- 📱 Fully responsive

**Everything works out of the box** — just run `npm run dev` and see it in action.

## 🛠️ Features

| Feature | Description |
|---------|-------------|
| **Auto Node.js Install** | Script offers to install Node.js if missing |
| **Folder Conflict Detection** | Prompts for new name if folder exists |
| **Tailwind v4** | Latest version with new `@import` syntax |
| **No Browser Interruption** | Script completes fully before you open the browser |
| **Cross-Platform** | Works on macOS, Linux, and Windows |
| **Clean Output** | Removes unused boilerplate files |

## 📦 What Gets Installed

```json
{
  "dependencies": {
    "react": "^19.x",
    "react-dom": "^19.x"
  },
  "devDependencies": {
    "@vitejs/plugin-react": "^4.x",
    "vite": "^6.x",
    "tailwindcss": "^4.x",
    "@tailwindcss/postcss": "^4.x",
    "postcss": "^8.x"
  }
}
```

## 🎨 Tailwind v4 Setup

The script configures Tailwind v4 with the new simplified setup:

**postcss.config.js**
```js
export default {
  plugins: {
    "@tailwindcss/postcss": {},
  },
};
```

**src/index.css**
```css
@import "tailwindcss";
@source "../";
```

No `tailwind.config.js` needed — Tailwind v4 auto-detects your content.

## 🔧 After Setup

```bash
# Navigate to your project
cd my-app

# Start dev server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## 💡 Tips

### Adding Custom Fonts

```css
/* src/index.css */
@import "tailwindcss";
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap');

body {
  font-family: 'Inter', sans-serif;
}
```

### Adding Plugins

```bash
npm install -D @tailwindcss/typography @tailwindcss/forms
```

```css
/* src/index.css */
@import "tailwindcss";
@plugin "@tailwindcss/typography";
@plugin "@tailwindcss/forms";
```

### Dark Mode

Tailwind v4 supports dark mode out of the box:

```jsx
<div className="bg-white dark:bg-slate-900">
  <h1 className="text-black dark:text-white">Hello!</h1>
</div>
```

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repo
2. Create a feature branch (`git checkout -b feature/amazing`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing`)
5. Open a Pull Request

## ☕ Support

If this saved you time, consider buying me a coffee:

<a href="https://ko-fi.com/alejandrodlrocha">
  <img src="https://img.shields.io/badge/Ko--fi-Support-ff5e5b?style=for-the-badge&logo=ko-fi&logoColor=white" alt="Ko-fi" />
</a>
<a href="https://www.buymeacoffee.com/alejandrodlrocha">
  <img src="https://img.shields.io/badge/Buy%20Me%20a%20Coffee-Support-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black" alt="Buy Me a Coffee" />
</a>

## 📄 License

MIT © [Alejandro de la Rocha](https://nolti.io)

---

<div align="center">

**Built by a developer who got tired of copying config files.**

[⬆ Back to top](#-reactvitetailwindcom)

</div>
