# 🃏 Name Card Workshop — Session Playbook
**Format:** 30-minute team activity  
**Stack:** Vite + Vanilla JS + GSAP  
**Goal:** Each designer builds a personal name card that represents their personality — color, type, animation and all.

---

## Pre-Made Starter Folder

Set this up ahead of time and share as a zip (with `node_modules` already inside — no `npm install` required on the day).

```
name-card-starter/
├── index.html
├── main.js
├── style.css
├── package.json
├── node_modules/
└── README.md
```

**README.md**
```
1. Open your terminal in this folder
2. Run: npm run dev
3. Open: http://localhost:5173
```

**index.html**
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <link rel="stylesheet" href="/style.css" />
    <title>Name Card</title>
  </head>
  <body>
    <div class="card" id="card">
      <!-- Your name card goes here -->
    </div>
    <script type="module" src="/main.js"></script>
  </body>
</html>
```

**main.js**
```js
import gsap from 'gsap';

// GSAP is ready. Ask Claude to animate anything inside #card.
// Example: gsap.from("#card", { opacity: 0, y: 40, duration: 1 });
```

**style.css**
```css
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

:root {
  --color-bg: #0f0f0f;
  --color-accent: #ff4d00;
  --font-main: 'Inter', sans-serif;
}

body {
  background: var(--color-bg);
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}
```

---

## Claude Prompt Template

Share this with designers to fill in before prompting. The more specific, the better the output.

```
I have a Vite + Vanilla JS project with GSAP already imported in main.js.
Build me a personal name card inside the existing #card div.
Write the HTML into index.html, CSS into style.css, and animations into main.js.

Here's what I want:
- My name: [Name]
- My role: [Role]
- Vibe / mood: [e.g. "dark and minimal, like a luxury brand"]
- Color palette: [e.g. "near-black background, electric lime accent"]
- Typography feeling: [e.g. "oversized serif name, tiny mono for the details"]
- Animation on load: [e.g. "each letter of my name drops in one by one"]
- Animation on hover: [e.g. "the card tilts in 3D as my cursor moves across it"]
- One extra detail: [e.g. "a slow animated gradient behind everything"]

Use GSAP for all animations. Make it feel like a real portfolio piece, not a template.
```
