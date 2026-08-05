# College Event Hub — EventHub

A modern, frontend-only college event discovery and registration website built with HTML, CSS, and vanilla JavaScript. No frameworks or build tools required.

## 🚀 Core Features

- **Event Catalog**: Browse upcoming campus events with titles, dates, descriptions, and poster images.
- **Featured Carousel**: Highlighted “Trending Now” events with prev/next navigation.
- **Event Details**: Dedicated detail view with venue, time, organizer, and full description.
- **Registration Modal**: Demo registration form (name, email, phone, department, event select) with validation.
- **Live Countdown**: Hero timer counting down to the next upcoming event.
- **Toast Notifications**: Success feedback after submitting a registration.
- **Sticky Navbar**: Smooth scrolling, active link highlighting, and a collapsible mobile menu.
- **Responsive Design**: Works on desktop and mobile.

## 🏃 Quick Start

### 1. Open the project folder

```bash
cd collegeeventhub
```

### 2. Start a local server

**Option A — Python (recommended)**

```bash
python -m http.server 3000 --bind 127.0.0.1
```

**Option B — Node.js**

```bash
npx serve -l 3000
```

**Option C — VS Code / Cursor Live Server**

Install the **Live Server** extension → right-click `index.html` → **Open with Live Server**.

### 3. Open the site

Visit the URL below in your browser.

## 📊 Access URLs

| Service   | URL                                      |
|-----------|------------------------------------------|
| Website   | http://127.0.0.1:3000                    |
| Website   | http://localhost:3000 *(Node / Live Server)* |

Stop the server with `Ctrl + C` in the terminal.

> You can also open `index.html` directly via **File → Open**, but a local server is preferred so paths and browser APIs behave consistently.

## 📁 Project Structure

```
collegeeventhub/
├── index.html   # Page markup, sections, registration modal, footer
├── style.css    # Layout, themes, animations, and responsive styles
├── events.js    # Event data (titles, dates, venues, images, etc.)
├── script.js    # Rendering, carousel, countdown, modal, and UI logic
└── README.md
```

## 🛠️ Tech Stack

- HTML5
- CSS3 (custom properties, gradients, animations, responsive layout)
- Vanilla JavaScript
- Font Awesome & Google Fonts (CDN)

## ✏️ Customizing

| What                | Where                                |
|---------------------|--------------------------------------|
| Events / featured   | `events` array in `events.js`        |
| Colors & layout     | CSS variables in `style.css` (`:root`) |
| Page sections       | `index.html`                         |
| UI behavior         | `script.js`                          |

Set `featured: true` on an event in `events.js` to show it in the Trending Now carousel.

## 📝 Notes

- Registration is a UI demo only — no backend, database, or API is included.
- Form submissions show a success toast; data is not stored or sent anywhere.
- Contact details in the footer are placeholders for the demo.
- Event images are loaded from Unsplash URLs; an internet connection is required to display them.
