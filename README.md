# Professional Portfolio Website - Yashi Sahu

A modern, responsive, and minimal portfolio website built specifically for a Computer Science Engineering student looking for internships and software developer roles.

## 🚀 Live Preview & Deployment
The website is fully compatible with **GitHub Pages** (pure HTML5, CSS3, and Vanilla JavaScript).

To deploy:
1. Push this entire folder to a public repository on GitHub.
2. Go to the repository **Settings** tab.
3. Scroll down to **Pages** in the left sidebar.
4. Select `main` branch (and `/ (root)` folder) as the source, and click **Save**.
5. Wait a few minutes, and your site will be live at `https://<your-username>.github.io/<your-repo-name>/`.

---

## 📂 Project Structure
```
Portfolio/
│
├── index.html          # Main HTML markup with SEO metadata & semantic elements
├── style.css           # Custom CSS variables, light/dark themes, animations, & styling
├── script.js           # Interactive components (Typing, Scroll reveals, Theme switches)
├── assets/
│   ├── images/         # Placeholders & graphics
│   ├── icons/          # Vector SVG icons
│   └── resume.pdf      # Placeholder PDF file for downloading resume
└── README.md           # Project guide & notes
```

---

## 🛠️ Customization Guide

### 1. Update Your Resume
- Replace the dummy `assets/resume.pdf` file with your actual PDF resume. Make sure to keep the filename as `resume.pdf` (or update the filename reference in `index.html` on line 75).

### 2. Update Your Contact details and Social Profiles
Search for the following details in `index.html` and replace them with your own links:
- Email: `sahuyashi38@gmail.com`
- Phone: `8924826576`
- GitHub Link: `https://github.com/sahuyashi38`
- LinkedIn Link: `https://linkedin.com/in/yashi-sahu`

### 3. Setup Custom Profile Picture
To show your actual photo instead of the SVG graphic in the Hero section:
1. Move your image file (e.g. `yashi.jpg`) into the `assets/images/` directory.
2. In [index.html](file:///c:/Users/sahuy/OneDrive/Desktop/front-end%20Project/index.html), go to the `<div class="hero-illustration">` block (around line 96) and replace the SVG content inside `<div class="profile-img-container">` with:
   ```html
   <img src="assets/images/yashi.jpg" alt="Yashi Sahu Profile Picture" style="width: 100%; height: 100%; object-fit: cover;">
   ```

### 4. Enable Live GitHub Stats
The statistics section is already linked to the GitHub username `sahuyashi38` using the GitHub Readme Stats API.
- If you change your GitHub username in the future, open `index.html`, scroll to the **GitHub Statistics** section (around line 431), and change the `username=sahuyashi38` parameter in the `img` URLs to your new username.

---

## ✨ Features Included
- **Sticky Navigation**: Slides in with active menu highlighting (scrollspy).
- **Dark/Light Mode**: Full customization theme switch, persisting selection via `localStorage`.
- **Text Typing Animation**: Dynamically cycles roles in the Hero section.
- **Scroll Reveals**: Intersection Observer triggering fade-ins on scroll.
- **Animated Skill Bars**: Progress fills up dynamically when the skills section scrolls into view.
- **Contact Form Validation**: Full front-end verification displaying a custom animated validation toast.
- **Mobile Responsive Layout**: Uses flex/grid scaling down to hamburger drawers on mobile devices.
