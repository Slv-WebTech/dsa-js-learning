<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=32&pause=1000&color=22D3EE&center=true&vCenter=true&width=700&lines=DSA+%2B+JavaScript+Learning+Journey+%F0%9F%9A%80;Learn.+Code.+Test.+Revise.+Repeat." alt="Typing SVG" />

<br/>

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap_5-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)

<br/>

> **A personal DSA + JavaScript study dashboard** — each concept gets its own card with  
> a theory panel, live code block, and expected output, all in one dark-themed interface.

<br/>

[✦ Live Demo](#) &nbsp;·&nbsp; [✦ Add a Topic](#how-to-add-a-topic) &nbsp;·&nbsp; [✦ Topics Covered](#topics-covered)

</div>

---

## ✨ Features

| Feature | Description |
|---|---|
| 📚 **Topic Cards** | Each concept has its own full-width section with Concept, Code & Output panels |
| 🏷️ **Chip Navigation** | Click any chip to instantly filter to that topic — no scrolling |
| ➕ **Add Topic Form** | Fill a modal form → new card appears instantly, no HTML editing |
| 💾 **Save to JSON** | Uses the File System Access API to write `topics.json` directly to disk |
| 📂 **Load from JSON** | Pick your saved `topics.json` and reload all topics in one click |
| 🔔 **Toast Notifications** | Confirms every save, load, and add action |
| 🌙 **Dark UI** | Glassmorphism-inspired dark theme with gradient accents |

---

## 🗂️ Project Structure

```
dsa-js-learning/
│
├── index.html        ← Main app (topics data + renderer + form logic)
├── style.css         ← All styles (dark theme, chips, modal, toast)
├── Algorithms.js     ← Personal practice file (your scratch pad)
└── topics.json       ← Auto-generated when you click 💾 Save JSON
```

---

## 🚀 Getting Started

### 1 · Clone the repo

```bash
git clone git@github.com:Slv-WebTech/dsa-js-learning.git
cd dsa-js-learning
```

### 2 · Open in browser

No build step, no dependencies. Just open `index.html` directly:

```bash
# Option A — open directly (chips + cards work, file save uses download fallback)
start index.html

# Option B — serve locally (enables full File System API for direct JSON write)
npx serve .
# or with VS Code → install Live Server → right-click index.html → Open with Live Server
```

### 3 · Start learning

- All **17 prerequisite topics** are pre-loaded on first visit
- Your data persists automatically in `localStorage`
- Click **💾 Save JSON** once to write `topics.json` to your project folder
- From then on: **📂 Open JSON** → study → add → save

---

## 📖 How to Add a Topic

### Option A — Form (recommended)

1. Click **＋ Add Topic** in the chip bar
2. Fill in Title, Concept (HTML allowed), Code, Output/Notes
3. Hit **Save Topic** — the card appears instantly
4. Click **💾 Save JSON** to persist it to `topics.json`

### Option B — Edit the JSON file

Open `topics.json` and add an entry to the array:

```json
{
  "title": "Your Topic Title",
  "concept": "Explanation with <strong>highlights</strong>.<br><br><strong>Key 1</strong> → what it means",
  "code": "// your code here\nconsole.log('hello');",
  "output": "hello\n✔ key takeaway"
}
```

---

## 📚 Topics Covered

### 🟡 JavaScript Fundamentals

| # | Topic | Key Concepts |
|---|---|---|
| 1 | **var vs let vs const** | Scope, hoisting, TDZ, block vs function scope |
| 2 | **Sum of Two Numbers** | `+` operator, type coercion, `Number()`, `parseInt()` |
| 3 | **if / else — Conditional Logic** | `===` vs `==`, comparison operators, strict equality |
| 4 | **Data Types** | Primitives vs objects, `typeof`, `Array.isArray()` |
| 5 | **Type Conversion** | Implicit coercion, explicit conversion, truthy/falsy values |
| 6 | **Loops** | `for`, `while`, `for...of`, `for...in`, `break`, `continue` |
| 7 | **Functions** | Declaration, expression, arrow functions, default params |
| 8 | **Arrays — Basics & Core Methods** | `push`, `pop`, `shift`, `unshift`, `slice`, `splice`, `sort` |
| 9 | **Array Methods** | `map`, `filter`, `find`, `findIndex`, `reduce`, `some`, `every` |
| 10 | **Objects — Key-Value Pairs** | Dot/bracket notation, `Object.keys/values/entries`, frequency counter |
| 11 | **Strings & String Methods** | `slice`, `split`, `includes`, `replace`, char array trick |
| 12 | **Destructuring & Spread / Rest** | Array/object destructuring, `...` spread, `...` rest, swap trick |
| 13 | **Ternary & Short-circuit** | `? :`, `&&`, `\|\|`, `??` nullish coalescing, `?.` optional chain |
| 14 | **Switch Statement** | `case`, `break`, fall-through, object map alternative |
| 15 | **Scope & Closures** | Global/function/block scope, closure, memoization pattern |
| 16 | **Math Object** | `floor`, `ceil`, `abs`, `max`, `min`, `sqrt`, `random` |

### 🔵 DSA Foundations

| # | Topic | Key Concepts |
|---|---|---|
| 17 | **Big O Notation** | O(1), O(log n), O(n), O(n²), time vs space complexity |

---

## 🎨 UI Preview

```
╔══════════════════════════════════════════════════════════════════╗
║         DSA + JavaScript Learning Journey 🚀                    ║
║    Learn → Code → Test → Revise → Repeat                        ║
╠══════════════════════════════════════════════════════════════════╣
║  [All Topics] [var vs let] [Loops] [Functions] ...              ║
║                               [📂 Open JSON] [💾 Save] [＋ Add] ║
╠══════════════════════════════════════════════════════════════════╣
║  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐ ║
║  │ 💡 Concept      │  │ 📄 Code         │  │ 🖥 Output       │ ║
║  │                 │  │                 │  │                 │ ║
║  │ Theory +        │  │ Live JS         │  │ Expected        │ ║
║  │ key points      │  │ code sample     │  │ result +        │ ║
║  │ with highlights │  │                 │  │ tips            │ ║
║  └─────────────────┘  └─────────────────┘  └─────────────────┘ ║
╚══════════════════════════════════════════════════════════════════╝
```

---

## 🛠️ Tech Stack

- **HTML5** — semantic structure, no frameworks
- **CSS3** — custom dark theme, glassmorphism, CSS transitions
- **Bootstrap 5** — grid layout only (`col-md-4`, `row`, `g-*`)
- **Vanilla JavaScript** — DOM manipulation, File System Access API, localStorage
- **File System Access API** — direct read/write to `topics.json` (Chrome / Edge 86+)

---

## 💡 Tips

- **Filter + study**: click a chip → full-screen view of that one topic
- **Concept HTML**: in the form, you can use `<strong>`, `<br>`, `<p>`, `<code>` tags
- **Backup**: after every session, click 💾 Save JSON — your file is your backup
- **Restore**: moved to a new machine? Clone repo, open page, click 📂 Open JSON, pick `topics.json`
- **Practice code**: write your solutions in `Algorithms.js` — it's your scratch pad

---

## 📄 License

MIT — use it, fork it, learn from it.

---

<div align="center">

Made with 💙 while learning DSA with JavaScript

**[⬆ Back to top](#)**

</div>
