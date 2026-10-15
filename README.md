# Interactive Web Apology 🌸

A responsive, romantic, and playful single-page apology web application crafted with HTML5 Canvas, CSS3, and vanilla JavaScript. Features animated floating hearts, an interactive dodging "No" button, an evolving heart tree canvas animation, background music, and an optional email webhook confirmation.

---

## ✨ Features

- **💌 Typed Apology Message**: Sincere typed-out message that introduces the apology smoothly.
- **🏃‍♂️ Playful Evasive "No" Button**: The "No" button dynamically darts away across the screen when clicked or tapped, cycling through pleading captions while scaling the "Yes" button larger.
- **🌳 Blooming Heart Tree**: Upon clicking "Yes", a procedural canvas animation dynamically grows a branching tree blooming with vibrant pink heart blossoms and falling petals accumulating at the base.
- **🎵 Romantic Background Music**: Plays ambient audio (`hareya.mp3`) starting on user interaction.
- **📜 Timed Apology Note**: Sequential apology promises revealed line-by-line synchronized with the animation.
- **📬 Instant Email Alerts**: Integrates FormSubmit to notify you immediately via email when "Yes" is clicked, including how many times they tried to click "No".
- **📱 Fully Responsive**: Fluid typography and layout designed to work seamlessly across mobile, tablet, and desktop viewports with reduced-motion support.

---

## 📁 Project Structure

```text
INTERACTIVE-WEB-APOLOGY-1/
├── index.html       # Core application (markup, styles, canvas & logic)
├── hareya.mp3       # Background audio track
├── README.md        # Project documentation
└── .gitignore       # Git ignore rules
```

---

## 🚀 Running Locally

No compilers, node modules, or build steps required. You can serve the directory with any local static server:

**Using Python:**
```powershell
python -m http.server 8000
```
Then open [http://localhost:8000](http://localhost:8000) in your browser.

**Using VS Code:**
Right-click `index.html` and select **"Open with Live Server"**.

---

## ⚙️ Customization

You can easily personalize the entire experience by editing the `CONFIG` object inside `index.html`:

```javascript
const CONFIG = {
  herName: "Name",
  notifyEmail: "your-email@example.com", // Set to "" to disable email alerts
  title: "A personal title",
  message: "Your heartfelt typed message here...",
  noLines: [
    "Are you sure?", "Please think again…", "I'm really sorry",
    "Pretty please?", "The button is running away, just say yes",
    "You can't catch it!", "I'll never forget again", "Last chance… say yes"
  ],
  yesSub: "A sweet subtitle after yes",
  apologyLines: [
    "First promise or line...",
    "Second line...",
    "You mean so much to me."
  ],
  apologyLineInterval: 1.8
};
```

---

## 🌐 Deploying to GitHub Pages

1. Navigate to your repository on GitHub: `https://github.com/subhranshunayak69-lab/INTERACTIVE-WEB-APOLOGY-1`
2. Go to **Settings** &rarr; **Pages** (under *Code and automation*).
3. Under **Build and deployment**:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` &amp; `/ (root)` folder.
4. Click **Save**.
5. Your interactive site will be live at:
   `https://subhranshunayak69-lab.github.io/INTERACTIVE-WEB-APOLOGY-1/`

