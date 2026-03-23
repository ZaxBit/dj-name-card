# Claude Code Design Jam - Name Card Workshop

[Workshop Deck](https://www.figma.com/deck/w5MCp6cYHFYFGV43jeI37e) | 
[Workshop Recording](https://drive.google.com/file/d/1t7arONxcT845hxZn5nqMGUMMX_ZGXYKm/view)

---

## Setup

### 1. Get the code

Open Cursor, then:

**File → New Window → Clone Git Repository**

Paste this URL:
```
https://github.com/ZaxBit/dj-name-card
```

### 2. Check Node.js

Open the terminal in Cursor (`⌘J`) and run:
```
node -v
```

You need **v18 or higher**. If the command is not found or the version is too low:
→ https://nodejs.org/en/download (download the **LTS** version)

### 3. Start the dev server

In the terminal (`⌘J`):
```
npm install
npm run dev
```

Then open: http://localhost:5173

You'll see a placeholder card. That's your starting point.

---

## Project structure

```
index.html   — the card lives inside <div id="card">
style.css    — global styles and CSS custom properties
main.js      — GSAP is imported here; add your animations
```

---

## Using Claude to build your card

Need help getting started? Prompt starters: https://djcard2026.figma.site

Or fill in this template and paste it into Claude:

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

---

## Share your results!  

Share it with me in #design-output or #claude-code-community!

Here's mine!  
![Adobe Express - dj-card-demo](https://github.com/user-attachments/assets/5aae4000-8c6f-4a2a-a38a-92a827056c36)


