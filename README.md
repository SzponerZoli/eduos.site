# eduOS Landing Page

**eduOS** is a free, open-source, immutable operating system built on Fedora Atomic, specifically designed for educational institutions. This repository contains the source code for the project's minimalist, high-performance landing page.

## ✨ Features

* **Minimalist & Modern:** Clean, dark-themed, distraction-free design built for scannability.
* **Profile Showcases:** Clear grid breakdown of the different machine profiles (Base, Student, Presentation, Teacher).
* **Pure CSS Tooltips:** Dynamic "Coming Soon" tooltips built with native Tailwind utility classes (no JS overhead).
* **Smooth Scrolling:** Seamless anchor-link navigation directly to the project roadmap.

## 🛠️ Tech Stack

* **HTML5** – Clean, semantic markup.
* **Tailwind CSS v4** – Utility-first CSS framework handling typography, responsive grids, animations, and custom theme variables via native CSS `@theme`.

## 🚀 Getting Started

Since this is a lightweight frontend landing page, no complex build steps or installations are required.

1. Clone the repository:
   ```bash
   git clone https://github.com/SzponerZoli/eduOS.git
   ```

## 🛠️ Local Development

Since the project uses **Tailwind CSS v4**, you need the CLI to watch and build the production CSS locally.

### 1. Install Dependencies
Install the required Tailwind CLI development tools:
```bash
npm install
```

### 2. Start Development Watcher
Run this command while editing. It will watch your `index.html` and `input.css` files and recompile the CSS instantly on every save:
```bash
npx @tailwindcss/cli -i ./input.css -o ./css/style.css --watch
```

### 3. Build for Production
Before committing or testing final performance, compile and heavily optimize/minify the stylesheet to get that 100% Lighthouse score:
```bash
npx @tailwindcss/cli -i ./input.css -o ./css/style.css --minify
```

## 🌐 Deployment

This landing page is deployed on **Cloudflare Pages**. Every time you push to the `main` branch, Cloudflare automatically pulls the changes and uses the `@tailwindcss/cli` build command to compile the fresh production styles.
```