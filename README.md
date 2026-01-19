# AIM-Lab Website | RBCCPS, IISc

The official website for the **Artificial Intelligence & Cyber-Physical Systems (AIM) Lab**, located at the Robert Bosch Centre for Cyber-Physical Systems (RBCCPS), Indian Institute of Science (IISc), Bangalore.

This repository contains the source code for a modern, responsive, and interactive lab portfolio website designed to showcase research, publications, projects, and team members.

## 🚀 About the Lab

**AIM-Lab** focuses on the intersection of **Machine Learning**, **Internet of Things (IoT)**, and **Sustainability**. Led by **Prof. Pandarasamy Arjunan**, the lab aims to build data-driven solutions that solve real-world challenges in smart built environments, energy sustainability, and cyber-physical systems.

## ✨ Key Features

* **Interactive Hero Section**: Features a canvas-based network graph animation, typewriter text effect, and animated statistic counters (Publications, Projects, Members).
* **Theme System**: Native **Dark Mode** and **Light Mode** support with a toggle switch, using CSS variables for easy color management.
* **Research Showcase**:
    * **Themes Grid**: Highlighted research pillars (Data Science, Energy, IoT).
    * **Methodologies**: Interactive grid showing core technical approaches.
    * **Projects**: Visual cards with hover zoom effects for active projects.
* **Publications**: Clean list layout with expandable `<details>` for abstracts and direct PDF links.
* **Team Section**: Professional profile cards with side-by-side social links (Scholar, LinkedIn, GitHub, Email).
* **Dynamic Elements**:
    * **Timeline**: Vertical timeline for recent news and updates.
    * **Gallery**: Filmstrip-style image gallery for lab facilities and life.
    * **Interactive Image**: "Mission" section with dynamic border effects.
* **Responsive Design**: Fully optimized for desktops, tablets, and mobile devices.

## 🛠️ Technologies Used

* **HTML5**: Semantic structure.
* **CSS3**: Custom properties (variables), Flexbox, CSS Grid, and advanced animations (keyframes, transitions).
* **JavaScript (Vanilla)**:
    * `IntersectionObserver` for scroll animations and counters.
    * Canvas API for the network background.
    * Local Storage for saving theme preferences.
* **Icons**: RemixIcon, FontAwesome, and Academicons.
* **Fonts**: Google Fonts (Poppins).

## 📂 Project Structure

```text
AIMLab/
│
├── index.html          # Main landing page (Single Page Application structure)
├── styles.css          # Global styles, variables, and responsive media queries
├── script.js           # Logic for animations, theme toggle, and UI interactions
├── README.md           # Project documentation
│
├── assets/
│   └── img/            # Images (Logos, Team photos, Project thumbnails, UI assets)
│       ├── iisc-logo.png
│       ├── anomaly.png
│       ├── speaker_pandarasamy.jpg
│       └── ...

## ⚙️ Setup & Usage

Since this is a static website, it does not require a complex backend server. You can run it locally or host it on any static site provider (GitHub Pages, Netlify, Vercel).

### 1. Cloning the Repository
Open your terminal or command prompt and run:

```bash
git clone https://github.com/your-username/AIM-Lab-Website. git
cd AIM-Lab-Website
```

### 2. Running Locally
You can simply double-click `index.html` to open it in your browser.

**Recommended Method (VS Code):**

1. Open the folder in VS Code. 
2. Install the Live Server extension.
3. Right-click `index.html` and select "Open with Live Server".

This ensures all assets, fonts, and scripts load correctly without CORS issues.

## 🎨 Customization Guide

### 1. Changing Colors
The entire color scheme is managed via CSS variables at the top of `styles.css`.

```css
:root {
  --primary: #4299e1;       /* Main Brand Blue */
  --primary-dark: #3182ce;  /* Darker Blue for hover states */
  --accent:  #ff4c29;        /* Accent Orange */
  --bg-light: #f8fafc;      /* Light Mode Background */
  /* ... */
}
```

### 2. Updating Content

- **News/Updates**: Edit the HTML under the `<section id="updates">` tag in `index.html`.

- **Stats Counters**: Update the numbers in the Hero section by changing the `data-count` attribute:

```html
<div class="hero-stat-number stat-number" data-count="50">0</div>
```

- **Typewriter Text**: Edit the `typewriterTexts` array in `script.js` to change the rotating text in the hero section:

```javascript
const typewriterTexts = [
    "Machine Learning",
    "Internet of Things",
    "Sustainability"
];
```

### 3. Adding Publications
To add a new publication, copy the existing `.pub-card` HTML block in `index.html` and paste it within the `.publications-wrapper` div.

## 📬 Contact

**Prof. Pandarasamy Arjunan**

- **Email**: samy@iisc.ac.in
- **Address**: Room No: 215, IDR Building, RBCCPS, IISc, Bangalore - 560012.

## 📄 License

© 2026 AIM-Lab, Indian Institute of Science. All rights reserved. 
