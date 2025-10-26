# Logic Legion | FTC Team 28874 Official Site

🤖 **Logic Legion** is an FTC (FIRST Tech Challenge) robotics team based in Apex, North Carolina, and powered by the **Apex Maker Club**. Our mission is to inspire creativity, teamwork, and a passion for robotics by designing, building, and programming unique robots that are fit for competitions.

This repository hosts the official team website, which serves as a central hub for our robot showcase, team information, foundation, and sponsor acknowledgments.

## 🚀 Quick Start

This website is a **single-page application** built primarily with **vanilla HTML** and the **Tailwind CSS CDN**, making it extremely easy to deploy.

### 1. Requirements

You only need a modern web browser to view the site and a text editor to modify the source code (`index.html`).

### 2. Local Development

Since the site is a single HTML file with no build step, you can view it locally by:

1.  **Cloning the repository:**
    ```bash
    git clone github.com/Hrishaan1/ftc28874portfolio
    cd logic-legion-site
    ```
2.  **Opening the file:** Double click `index.html` to open it directly in your web browser, or use a simple local server extension in your editor (like VS Code's Live Server).

## 🛠️ Technology Stack

* **HTML5:** The core structure of the single-page application.
* **Tailwind CSS (CDN):** Used for styling, providing utility-first classes for a modern, dark, neon-themed aesthetic without a dedicated build step.
* **Vanilla JavaScript:** Used for interactive elements like the mobile navigation toggle, smooth scrolling, element visibility transitions, and the administrative control for the Sponsors section.

## 🧩 Development notes

The site's JavaScript is now kept in a single external file for easier maintenance:

- Location: `js/main.js`
- How it's loaded: the script is included near the end of `index.html` right before `</body>` as `<script src="js/main.js"></script>` so it runs after the DOM is available.

Local testing / serving:

1. From the project root you can use Python's simple HTTP server:

```bash
# Python 3
python3 -m http.server 8000

# then open http://localhost:8000 in your browser
```

2. Or use an editor extension such as VS Code Live Server.

Deployment notes:

- If you deploy this repository to a static host (GitHub Pages, Netlify, Vercel, etc.) the `js/` folder will be deployed with the site by default. No build step is required.
- If you plan to add a strict Content Security Policy (CSP), allow the external script (`js/main.js`) or inline the parts that need to run under your policy.

## ⚙️ Customization and Configuration

### Tailwind Colors

The site uses a custom dark/neon color scheme defined within the `<script>` tag in the `<head>`:

```javascript
tailwind.config = {
  theme: {
    extend: {
      colors: {
        bg: '#060818',       // Main dark background
        'bg-2': '#071033',   // Secondary dark background (used in cards/sections)
        neon: '#00fff6',     // Primary accent color (cyan)
        accent: '#00fff6',   // Secondary accent color (cyan)
        'muted-blue': '#12223b'
      }
    }
  }
}
```

---

## ✅ To-Do List

Key files and content to update:

| File/Section | Purpose | Action Required |
| :--- | :--- | :--- |
| **`[Team Photo]`** | Hero section placeholder. | **Replace** the `<span>` with an `<img />` tag for the team photo. |
| **`#team` section** | Team member details. | **Update** `<span>Photo</span>` with `<img />` tags for member photos. |
| **`#robot` section** | Robot image | **Update** the CAD rendering after every update in the `<img />` tag in the `#robot` section. |
