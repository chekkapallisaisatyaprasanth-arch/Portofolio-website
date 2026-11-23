# Personal Portfolio Website 🚀

A modern, responsive, single-page personal portfolio website built with **pure HTML5 and CSS3 (Flexbox)**. Designed specifically for first-year B.Tech Computer Science & Engineering students for their Web Development subject activity, lab evaluation, and viva voce.

---

## 📌 Project Overview

- **Subject:** Web Development Activity / Lab
- **Author:** First-Year B.Tech CSE Student
- **Deadline:** 24th November EOD
- **Architecture:** Single-Page Architecture (SPA) using HTML anchor links
- **Constraints Met:** 100% Pure HTML5 & CSS3. **No JavaScript, no external frameworks (no Bootstrap, Tailwind), no CSS Grid.**

---

## 📁 Folder Structure

```text
portfolio/
├── index.html        # Main HTML file containing all 8 semantic sections
├── style.css         # Complete styling (CSS variables, Flexbox, media queries)
├── images/           # Local vector & placeholder assets
│   ├── profile.svg   # Student avatar illustration (replace with your photo)
│   ├── project1.svg  # Project 1 mockup graphic
│   ├── project2.svg  # Project 2 mockup graphic
│   └── project3.svg  # Project 3 mockup graphic
└── README.md         # Documentation & GitHub Pages deployment guide
```

---

## 🌟 Key Features

1. **Sticky Navigation Bar:** Uses `position: sticky; top: 0;` and smooth jump links (`#hero`, `#about`, `#skills`, `#projects`, `#achievements`, `#contact`).
2. **Hero / Profile Section:** Professional student introduction with call-to-action buttons, profile photo avatar, and clean gradient background.
3. **About Me & Quick Facts:** Biography narrative accompanied by responsive quick-fact cards (College, Year of Study, Location, Interests).
4. **CSS-Only Skill Progress Bars:** Skill cards featuring pure CSS progress bars with smooth gradient fills (`HTML5: 90%`, `CSS3: 80%`, `Flexbox: 85%`, `Git: 70%`), plus a "Currently Learning" section for academic coursework.
5. **Featured Projects Showcase:** 3 project cards with custom SVG preview illustrations, tech tags, and hover elevation effects (`transform: translateY(-8px)`).
6. **Milestones & Achievements:** Timeline cards highlighting entrance rank, web certifications, hackathons, and academic distinctions.
7. **Contact Information & Visual Form:** Functional email/phone/social anchor links alongside a styled frontend contact form layout.
8. **Responsive Design:** 100% mobile-friendly across desktop (1200px), tablet (768px), and mobile (375px) without horizontal scrolling.

---

## 🛠️ Built With

- **HTML5:** Semantic tags (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`) for accessibility and clean code structure.
- **CSS3:**
  - CSS Custom Properties (`:root` variables) for effortless theme customization.
  - Pure CSS **Flexbox** (`flex-direction`, `justify-content`, `align-items`, `flex-wrap`) for all layouts.
  - CSS Transitions (`transition: all 0.3s ease`) for interactive hover states.
  - Media Queries (`@media (max-width: 768px)` and `@media (max-width: 480px)`) for multi-device responsiveness.
- **Google Fonts:** `'Poppins', sans-serif` with robust system font fallbacks.

---

## ✏️ How to Customize for Yourself

All personalized fields in `index.html` are clearly marked with `<!-- EDIT: ... -->` comments:

1. **Your Name & Title:** Search for `<!-- EDIT: Your Full Name -->` in `index.html` and replace `John Doe`.
2. **Profile Photo:** 
   - Place your photo inside the `images/` folder (e.g., `images/my-photo.jpg`).
   - In `index.html`, change `src="images/profile.svg"` to `src="images/my-photo.jpg"`.
3. **College & Details:** Update the Quick Facts section under `#about` with your college name and location.
4. **Projects & Achievements:** Update the project titles, descriptions, and achievements with your own work.
5. **Contact Links:** Replace the placeholder email (`johndoe.student@example.com`), phone number, and LinkedIn/GitHub URLs with your actual links.
6. **Theme Colors (Optional):** Open `style.css` and change `--primary-color: #2563eb;` in the `:root` block to your favorite color (e.g. `#10b981` for emerald green or `#7c3aed` for purple).

---

## 🌐 Step-by-Step GitHub Pages Deployment Guide

Follow these steps to upload your code to GitHub and host your portfolio live for free:

### Method 1: Using the GitHub Web Interface (Easiest for Beginners)

1. **Log in to GitHub:** Go to [https://github.com](https://github.com) and log in to your account.
2. **Create a New Repository:**
   - Click the **"+"** icon in the top-right corner and select **New repository**.
   - **Repository name:** `personal-portfolio` (or `portfolio`).
   - Set visibility to **Public** (required for free GitHub Pages).
   - Leave "Initialize with README" **unchecked**.
   - Click **Create repository**.
3. **Upload Your Files:**
   - On the new repository page, click the link: **"uploading an existing file"**.
   - Drag and drop `index.html`, `style.css`, `README.md`, and the entire `images` folder into the upload box.
   - Wait for the files to finish uploading.
   - At the bottom, type a commit message (e.g. `Initial commit: personal portfolio`).
   - Click the green **Commit changes** button.
4. **Enable GitHub Pages:**
   - In your repository, click the **Settings** tab (gear icon at the top).
   - In the left sidebar, click on **Pages** (under the "Code and automation" section).
   - Under **Build and deployment**:
     - **Source:** select `Deploy from a branch`.
     - **Branch:** select `main` (or `master`) from the dropdown.
     - **Folder:** leave it as `/ (root)`.
   - Click **Save**.
5. **Get Your Live Link:**
   - Refresh the page after 1 to 2 minutes.
   - A banner will appear at the top:
     > **"Your site is live at https://&lt;your-username&gt;.github.io/personal-portfolio/"**
   - Click the link to open your live portfolio in your browser!

---

### Method 2: Using the Command Line (Git CLI)

If you have Git installed on your computer:

```bash
# 1. Initialize git in your project directory
git init

# 2. Add all files to the staging area
git add .

# 3. Create your first commit
git commit -m "feat: complete personal portfolio website"

# 4. Rename current branch to main
git branch -M main

# 5. Connect to your GitHub repository (replace with your repo URL)
git remote add origin https://github.com/<your-username>/personal-portfolio.git

# 6. Push your code to GitHub
git push -u origin main
```

After pushing, go to **Repository Settings -> Pages -> Deploy from branch -> Select `main` -> Save**.

---

## 🎓 Viva Voce Preparation Guide (Common Questions)

When explaining this project to your professor or external examiner, here are key answers you can give:

| Viva Question | Concise Answer to Give |
| :--- | :--- |
| **Why did you use Semantic HTML tags?** | Semantic tags (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`) clearly describe their meaning to both the browser and developers. They improve web accessibility (screen readers), SEO, and code maintainability over generic `<div>` tags. |
| **How does CSS Flexbox work in your project?** | Flexbox is a one-dimensional layout model. By setting `display: flex;` on a parent container, its direct children become flex items. I used `justify-content` to align items horizontally, `align-items` to align them vertically, and `flex-wrap: wrap;` so cards gracefully wrap onto new lines on smaller screens. |
| **Why are CSS Variables (`:root`) advantageous?** | CSS Custom Properties allow us to store repeated values like colors, font families, and border radii in one place. If the theme needs to change, modifying one variable updates the entire website instantly without searching through hundreds of lines. |
| **How is the navigation bar made sticky without JavaScript?** | I used `position: sticky; top: 0;` on `.navbar-header` with a higher `z-index: 1000;`. This tells the browser to keep the header fixed at the top once the user scrolls past its natural position. |
| **What does `scroll-behavior: smooth;` do?** | Placed on the `html` selector, it produces a smooth gliding transition when clicking anchor links (`href="#about"`), eliminating jarring instant jumps without needing JavaScript. |
| **What does the `<meta name="viewport" ...>` tag do?** | It instructs mobile browsers to render the page at the width of the physical device (`width=device-width`) with an initial scale of 1.0, enabling media queries to correctly scale the layout. |

---

## 📄 License & Academic Integrity

This project is built for educational purposes as part of the 1st-Year B.Tech CSE Web Development coursework. Feel free to use this as a learning reference!
