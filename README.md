# Logic Legion | FTC Team 28874 Official Site

🤖 **Logic Legion** is an FTC (FIRST Tech Challenge) robotics team based in Apex, North Carolina, and powered by the **Apex Maker Club**. Our mission is to inspire creativity, teamwork, and a passion for robotics by designing, building, and programming unique competition robots.

This repository hosts the official team website, which serves as a central hub for our robot showcase, team information, foundation, and sponsor acknowledgments.

## 🚀 Quick Start

This website is a **single-page application** built primarily with vanilla HTML and the **Tailwind CSS CDN**, making it extremely easy to deploy.

### 1. Requirements

You only need a modern web browser to view the site and a text editor to modify the source code (`index.html`).

### 2. Local Development

Since the site is a single HTML file with no build step, you can view it locally by:

1.  **Cloning the repository:**
    ```bash
    git clone [Your Repository URL Here]
    cd logic-legion-site
    ```
2.  **Opening the file:** Drag and drop `index.html` directly into your web browser, or use a simple local server extension in your editor (like VS Code's Live Server).

### 3. Deployment

Simply upload the `index.html` file and any linked assets (like `logiclegionlogo.jpg`, `robot.png`, team photos) to any web hosting service (e.g., GitHub Pages, Netlify, Vercel).

---

## 🛠️ Technology Stack

* **HTML5:** The core structure of the single-page application.
* **Tailwind CSS (CDN):** Used for styling, providing utility-first classes for a modern, dark, neon-themed aesthetic without a dedicated build step.
* **Vanilla JavaScript:** Used for interactive elements like the mobile navigation toggle, smooth scrolling, element visibility transitions, and the administrative control for the Sponsors section.

---

## ⚙️ Customization and Configuration

### A. Global Content & Assets

Key files and content to update:

| File/Section | Purpose | Action Required |
| :--- | :--- | :--- |
| **`logiclegionlogo.jpg`** | Header and Favicon logo. | **Replace** with the official team logo file. |
| **`robot.png`** | Hero and Robot section image. | **Replace** with a photo/render of the current season's robot. |
| **`[Team Photo]`** | Hero section placeholder. | **Replace** the `<span>` with an `<img />` tag for the team photo. |
| **`#about` section** | Team philosophy and competition goals. | **Edit** the placeholder text for philosophy and goals. |
| **`#team` section** | Team member details. | **Update** names, roles, and replace `<span>Photo</span>` with `<img />` tags for member photos. |
| **`#sponsors` section** | Sponsor logos and details. | **Replace** the placeholder SVG/text with high-resolution sponsor logos. |
| **Footer (Email)** | Contact information. | **Verify** the email address is current: `ftcteam28874@apexmakerclub.org`. |

### B. Tailwind Colors

The site uses a custom dark/neon color scheme defined within the `<script>` tag in the `<head>`:

```javascript
tailwind.config = {
  theme: {
    extend: {
      colors: {
        bg: '#060818',       // Main dark background
        'bg-2': '#071033',   // Secondary dark background (used in cards/sections)
        neon: '#00fff6',     // Primary accent color (cyan)
        accent: '#7c5cff',   // Secondary accent color (purple/indigo)
        'muted-blue': '#12223b'
      }
    }
  }
}