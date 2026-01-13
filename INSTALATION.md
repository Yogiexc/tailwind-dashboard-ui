# 🚀 Installation Guide - Tailwind Dashboard UI

Panduan lengkap setup project dari awal sampai running.

---

## ✅ Prerequisites

Pastikan sudah terinstall:

```bash
# Check Node.js (minimal v18)
node --version
# Output: v18.x.x atau lebih tinggi

# Check npm
npm --version
# Output: 9.x.x atau lebih tinggi
```

Jika belum ada, download dari [nodejs.org](https://nodejs.org/)

---

## 📦 Step 1: Create Project Folder

```bash
# Buat folder project
mkdir tailwind-dashboard-ui
cd tailwind-dashboard-ui
```

---

## 📝 Step 2: Initialize npm

```bash
# Initialize package.json
npm init -y
```

Output:
```json
{
  "name": "tailwind-dashboard-ui",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [],
  "author": "",
  "license": "ISC"
}
```

---

## 🎨 Step 3: Install Tailwind CSS v4

```bash
# Install Tailwind CSS v4 (next version)
npm install -D tailwindcss@next @tailwindcss/cli@next
```

**Note:** Kita pakai `@next` untuk Tailwind v4 (masih alpha/beta)

Output:
```
added 2 packages in 3s
```

---

## ⚙️ Step 4: Create Configuration Files

### 4.1 Create `tailwind.config.js`

```bash
# Create file
touch tailwind.config.js
```

Paste konten berikut:

```javascript
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ['./src/**/*.{html,js}'],
  darkMode: 'class',
  theme: {
    extend: {
      colors: {
        ocean: {
          50: '#f0f9ff',
          100: '#e0f2fe',
          200: '#bae6fd',
          300: '#7dd3fc',
          400: '#38bdf8',
          500: '#0ea5e9',
          600: '#0284c7',
          700: '#0369a1',
          800: '#075985',
          900: '#0c4a6e',
          950: '#082f49',
        },
        wine: {
          50: '#fdf4ff',
          100: '#fae8ff',
          200: '#f5d0fe',
          300: '#f0abfc',
          400: '#e879f9',
          500: '#d946ef',
          600: '#c026d3',
          700: '#a21caf',
          800: '#86198f',
          900: '#701a75',
          950: '#4a044e',
        },
        forest: {
          50: '#f0fdf4',
          100: '#dcfce7',
          200: '#bbf7d0',
          300: '#86efac',
          400: '#4ade80',
          500: '#22c55e',
          600: '#16a34a',
          700: '#15803d',
          800: '#166534',
          900: '#14532d',
          950: '#052e16',
        },
      },
    },
  },
  plugins: [],
}
```

### 4.2 Update `package.json` scripts

Edit `package.json`, tambahkan scripts:

```json
{
  "name": "tailwind-dashboard-ui",
  "version": "1.0.0",
  "description": "Modern dashboard UI using Tailwind CSS v4",
  "scripts": {
    "dev": "tailwindcss -i ./src/input.css -o ./dist/output.css --watch",
    "build": "tailwindcss -i ./src/input.css -o ./dist/output.css --minify"
  },
  "keywords": ["tailwind", "dashboard", "design-system"],
  "author": "",
  "license": "MIT",
  "devDependencies": {
    "@tailwindcss/cli": "^4.0.0-alpha.25",
    "tailwindcss": "^4.0.0-alpha.25"
  }
}
```

### 4.3 Create `.gitignore`

```bash
# Create file
touch .gitignore
```

Paste konten:

```
# Dependencies
node_modules/
package-lock.json

# Build output
dist/
*.css.map

# Environment
.env
.env.local

# IDE
.vscode/
.idea/
*.swp

# OS
.DS_Store
Thumbs.db

# Logs
*.log

# Temporary
*.tmp
.cache/
```

---

## 📁 Step 5: Create Project Structure

```bash
# Create folders
mkdir src
mkdir dist

# Create files
touch src/index.html
touch src/input.css
```

Struktur sekarang:
```
tailwind-dashboard-ui/
├── node_modules/
├── src/
│   ├── index.html
│   └── input.css
├── dist/
├── .gitignore
├── package.json
└── tailwind.config.js
```

---

## 🎨 Step 6: Create Source Files

### 6.1 Create `src/input.css`

Paste konten:

```css
@tailwind base;
@tailwind components;
@tailwind utilities;

/* Custom base styles */
@layer base {
  body {
    @apply bg-gray-50 dark:bg-gray-900 text-gray-900 dark:text-gray-100 transition-colors duration-200;
  }
}

/* Theme variants untuk Ocean theme */
.theme-ocean {
  --tw-ocean-primary: #0284c7;
  --tw-ocean-light: #38bdf8;
  --tw-ocean-dark: #0369a1;
}

.theme-ocean .sidebar-active {
  @apply bg-ocean-600;
}

.theme-ocean .btn-primary {
  @apply bg-ocean-600 hover:bg-ocean-700;
}

/* Theme variants untuk Wine theme */
.theme-wine {
  --tw-wine-primary: #c026d3;
  --tw-wine-light: #e879f9;
  --tw-wine-dark: #a21caf;
}

.theme-wine .sidebar-active {
  @apply bg-wine-600;
}

.theme-wine .btn-primary {
  @apply bg-wine-600 hover:bg-wine-700;
}

/* Theme variants untuk Forest theme */
.theme-forest {
  --tw-forest-primary: #16a34a;
  --tw-forest-light: #4ade80;
  --tw-forest-dark: #15803d;
}

.theme-forest .sidebar-active {
  @apply bg-forest-600;
}

.theme-forest .btn-primary {
  @apply bg-forest-600 hover:bg-forest-700;
}

/* Smooth transitions for theme changes */
@layer utilities {
  .transition-theme {
    @apply transition-all duration-300 ease-in-out;
  }
}
```

### 6.2 Create `src/index.html`

**Copy dari artifact yang sudah saya buat** - File lengkap dengan:
- Sidebar navigation
- Top navbar
- Stats cards
- Data table
- Theme switcher
- Responsive design
- Dark mode support

---

## 🏗️ Step 7: Build CSS

```bash
# Development mode (watch for changes)
npm run dev
```

Output:
```
Rebuilding...

Done in 45ms.
```

**Terminal akan tetap running** dan auto-rebuild saat ada perubahan.

---

## 🌐 Step 8: Open Dashboard

### Option 1: Direct Open (Simple)

```bash
# Buka file langsung di browser
# Windows: start src/index.html
# Mac: open src/index.html
# Linux: xdg-open src/index.html
```

### Option 2: Live Server (Recommended)

**Via VS Code:**
1. Install extension "Live Server"
2. Right-click pada `src/index.html`
3. Pilih "Open with Live Server"
4. Browser auto-open di `http://localhost:5500`

**Via CLI:**
```bash
# Install http-server globally (one time)
npm install -g http-server

# Run server
npx http-server src/ -p 3000

# Akses di browser:
# http://localhost:3000
```

---

## ✅ Step 9: Verify Installation

Dashboard harus:
- ✅ Tampil dengan sidebar & navbar
- ✅ Stats cards terlihat bagus
- ✅ Table dengan data
- ✅ Theme switcher berfungsi (Light/Dark/Ocean/Wine/Forest)
- ✅ Responsive di mobile (sidebar collapse)
- ✅ Smooth transitions

---

## 🐛 Troubleshooting

### Error: "Could not resolve value for theme function"

**Penyebab:** Custom colors belum didefinisikan di `tailwind.config.js`

**Solusi:**
```javascript
// Pastikan ada di tailwind.config.js
theme: {
  extend: {
    colors: {
      ocean: { /* ... */ },
      wine: { /* ... */ },
      forest: { /* ... */ },
    }
  }
}
```

### Error: "Cannot find module 'tailwindcss'"

**Penyebab:** Tailwind belum terinstall

**Solusi:**
```bash
npm install -D tailwindcss@next @tailwindcss/cli@next
```

### Dashboard tidak muncul / CSS tidak load

**Penyebab:** Path CSS salah di HTML

**Solusi:** Check di `index.html`:
```html
<!-- Pastikan path benar -->
<link rel="stylesheet" href="../dist/output.css">
```

### Theme switcher tidak jalan

**Penyebab:** JavaScript tidak load / error

**Solusi:** Check browser console (F12) untuk error messages

---

## 🎯 Production Build

Untuk deploy ke production:

```bash
# Build optimized CSS
npm run build
```

Output:
```
Rebuilding...

Done in 120ms.
```

Hasil:
```
dist/output.css
  - Minified
  - PurgeCSS applied
  - Only used utilities
  - ~8KB (vs 3.8MB dev)
```

---

## 📚 Next Steps

### Development Workflow

**Terminal 1:**
```bash
npm run dev  # Watch CSS changes
```

**Terminal 2:**
```bash
npx http-server src/ -p 3000  # Serve files
```

Edit `src/index.html` → CSS auto-rebuild → Browser auto-reload ✨

### Customization

**Add custom colors:**
```javascript
// tailwind.config.js
theme: {
  extend: {
    colors: {
      brand: {
        500: '#your-color'
      }
    }
  }
}
```

**Add custom components:**
```css
/* src/input.css */
@layer components {
  .btn-custom {
    @apply px-4 py-2 bg-brand-500 text-white rounded-lg;
  }
}
```

---

## 🎉 Success!

Dashboard sudah running! 🚀

Sekarang kamu bisa:
- ✅ Edit HTML untuk customize layout
- ✅ Add more components
- ✅ Customize theme colors
- ✅ Build production-ready CSS

---

## 📞 Need Help?

- Check `README.md` untuk dokumentasi lengkap
- Check `CONCEPTS.md` untuk deep dive concepts
- Check `QUICK_REFERENCE.md` untuk utility classes cheatsheet

**Happy coding! 💙**