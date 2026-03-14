# Nayan Sinha - Developer Portfolio

A modern, responsive, and visually impressive developer portfolio built using HTML, CSS, JavaScript, Three.js, and GSAP. 

## Features
- **Modern Dark/Light Theme**: Sleek UI with simple theme toggling.
- **Interactive 3D Background**: Built using Three.js with an accent color that follows mouse movement.
- **Scroll Animations**: Smooth entrance animations using GSAP and ScrollTrigger.
- **Contact Form**: Ready for integration with EmailJS.
- **Fully Responsive**: Optimized for desktop, tablet, and mobile.

## Project Structure
```text
portfolio/
├── index.html       # Main HTML structure
├── style.css        # Custom CSS variables, Layout, & Responsive Design
├── script.js        # ThreeJS, GSAP animations, theme logic, & mobile nav
└── assets/          # Directory for future images and icons
    ├── images/
    └── icons/
```

## How to Run Locally
1. Clone the repository or download the files.
2. Open the directory in your terminal.
3. If you have Python installed, you can start a simple server:
   ```bash
   python -m http.server 8000
   ```
   Or using Node.js/npx:
   ```bash
   npx serve
   ```
4. Open your browser and navigate to `http://localhost:8000` or the port provided by `npx serve`.

*(Alternatively, you can just open `index.html` directly in your browser, but due to browser security restrictions around ES modules/Canvas, running via a local server is recommended for the Three.js canvas to render correctly).*

## Setting up EmailJS for the Contact Form
1. Go to [EmailJS](https://www.emailjs.com/) and create a free account.
2. Add an Email Service (e.g., Gmail).
3. Create an Email Template.
4. Open `script.js` and locate the EmailJS configuration section.
5. Replace `YOUR_EMAILJS_PUBLIC_KEY`, `YOUR_SERVICE_ID`, and `YOUR_TEMPLATE_ID` with your actual keys from the EmailJS dashboard.
6. Uncomment the `emailjs.sendForm(...)` code block in `script.js`.

## Hosting on GitHub Pages (Free)
Follow these exact steps to host your portfolio online for free:

1. **Create a GitHub Repository:**
   - Go to [GitHub](https://github.com) and log in.
   - Click the **+** icon in the top right and select **New repository**.
   - Name it `Nayansinha2021.github.io` (this is a special repo name that tells GitHub to host it at that exact URL).
   - Make sure it's set to **Public** and click **Create repository**.

2. **Upload Your Files:**
   - On your computer, open your terminal/command prompt and navigate to your `portfolio` directory.
   - Run the following commands:
     ```bash
     git init
     git add .
     git commit -m "Initial commit of portfolio"
     git branch -M main
     git remote add origin https://github.com/Nayansinha2021/Nayansinha2021.github.io.git
     git push -u origin main
     ```
   *(Alternatively, you can manually upload the files via the GitHub web interface by clicking "upload an existing file" on the repository page).*

3. **Enable GitHub Pages (If not using the special repo name):**
   - If you named your repo something else (like just `portfolio`), go to the repository page on GitHub.
   - Click **Settings** > **Pages** (in the left sidebar).
   - Under "Build and deployment", select **Deploy from a branch**.
   - Select the `main` branch, keep the folder as `/ (root)`, and click **Save**.
   - Wait 1-2 minutes, and your site will be live!

4. Your portfolio will now be accessible online. Add this link to your resume and LinkedIn!
