# 🚀 Dipesh Bham - Interactive Personal Portfolio

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Web3Forms](https://img.shields.io/badge/Form_API-Web3Forms-0052FF?style=for-the-badge&logo=googlecloud&logoColor=white)](https://web3forms.com)
[![Status](https://img.shields.io/badge/Status-Live-success?style=for-the-badge)](https://dipeshbham.com.np/)

Welcome to the repository of **Dipesh Bham's Personal Portfolio**. This is a premium, cutting-edge, single-page web experience showcasing expertise in Full Stack Development, UI/UX Glassmorphism Design, and Graphic Design.

Built from scratch with **Vanilla CSS3** and **Modular ES6+ JavaScript**, this project highlights how rich aesthetics, smooth animations, and high performance can merge to deliver a premium user experience without bloated frameworks.

---

## ✨ Features

- **🌌 Dynamic Particle Canvas**: An interactive HTML5 Canvas background that responds to mouse movements, creating a cybernetic, connected-nodes visual effect.
- **🖼️ Cinematic Slideshow**: Full-screen background slideshow utilizing timed cross-fade CSS transitions for a dynamic environment.
- **⏱️ Smart Preloader**: Elegant spinning rings with text indicators that fade away smoothly after document loading is complete.
- **📱 Fluid Glassmorphic Design**: Sleek card components, floating overlays, and blurred background glows following modern glassmorphism design patterns.
- **🧭 Auto-Highlighting Navigation**: Sticky navbar with a responsive hamburger drawer (locking body scroll on open) and smart active-link highlights based on scroll position.
- **📊 Interactive Statistics & Skill Bars**: Dynamic counters that count up to targets and skill level meters that fill up automatically using `IntersectionObserver` when scrolled into view.
- **🎭 Typing Animation**: Interactive header typing effect showcasing diverse roles dynamically.
- **📁 Category-Based Project Filter**: Client-side filtering mechanism to sort projects (Web Apps, Full Stack, CLZ Projects) instantly.
- **✉️ Validated Contact Form**: Secure contact form with comprehensive live validation, responsive loaders, and direct email delivery using the **Web3Forms API**.
- **🎯 Custom Cursor Followers**: Visual indicator trail tracking the user's cursor across elements for heightened interactivity.
- **🔔 Premium Popup Ads**: Custom dismissable lead-generation modal to capture prospective client inquiries.

---

## 🛠️ Tech Stack

- **Structure**: Semantic HTML5
- **Styling**: Vanilla CSS3 (CSS Variables, Flexbox/Grid, `@keyframes` key animations, Glassmorphic blurs)
- **Logics**: ES6+ JavaScript (Intersection Observer API, Canvas 2D API, Fetch API)
- **Icons**: Font Awesome v6.4.0
- **Typography**: Google Fonts (Inter, Roboto, Outfit)
- **Form Delivery**: Web3Forms API

---

## 📂 Project Structure

```
├── assets/
│   └── images/
│       ├── bg1.jpg          # Slideshow background image 1
│       ├── bg2.JPG          # Slideshow background image 2
│       ├── bg3.jpg          # Slideshow background image 3 / Profile picture
│       ├── bhetly.webp      # Project mockup (Bhetly)
│       ├── hamrodera.png    # Project mockup (HamroDera)
│       └── webproject 1.png # Project mockup (aNepaliSewa)
├── index.html               # Main entry HTML file (SEO optimized, schema structured)
├── script.js                # Core interactive JavaScript logic
├── style.css                # Visual theme, transitions, glassmorphic layout styles
└── README.md                # Project documentation (this file)
```

---

## 🚀 Getting Started

### Prerequisites
To run this project locally, you don't need any complex framework compilers or dependencies. Just a browser!

### Running Locally
1. Clone this repository or download the files.
2. Open `index.html` in your favorite web browser directly.
3. *Recommended*: Use a local development server for the best performance and network feature support (e.g. VS Code's **Live Server** extension, or `npx browser-sync start --server --files "*"`).

---

## ⚙️ Configuration & Customization

### 1. Update Contact Form Email Destination
The contact form uses **Web3Forms**. To receive messages sent by users directly to your inbox:
1. Go to [Web3Forms](https://web3forms.com/) and register your email to get a free **Access Key**.
2. Open `script.js` and find the form submit handler (around line 288).
3. Replace the access key string with your new key:
   ```javascript
   formData.append('access_key', 'YOUR_WEB3FORMS_ACCESS_KEY_HERE');
   ```

### 2. Add or Edit Projects
To add more work cards, update the projects grid container in `index.html`. Format cards like this:
```html
<div class="project-card reveal" data-category="web|design|fullstack">
    <div class="project-img-wrapper">
        <img src="assets/images/your-project.png" alt="Description">
    </div>
    <div class="project-body">
        <h3 class="project-title">Project Name</h3>
        <p class="project-desc">Description of the project...</p>
        <div class="project-tech">
            <span class="tech-badge">HTML</span>
            <span class="tech-badge">CSS</span>
            <span class="tech-badge">JavaScript</span>
        </div>
        <div class="project-links">
            <a href="URL" class="project-link project-link-demo">Live Demo</a>
            <a href="URL" class="project-link project-link-code">Source</a>
        </div>
    </div>
</div>
```

### 3. Customize Background Slideshow
Update images under `assets/images/` or change the slideshow cycle time in `script.js` (currently set to 6 seconds / `6000`ms):
```javascript
setInterval(() => {
    bgSlides[cur].classList.remove('active');
    cur = (cur + 1) % bgSlides.length;
    bgSlides[cur].classList.add('active');
}, 6000); // <-- Adjust time interval here
```

---

## ☁️ Deployment

### GitHub Pages (Fastest)
1. Push this project to a GitHub repository.
2. Go to repository **Settings** -> **Pages**.
3. Under *Build and deployment*, set Source to **Deploy from a branch**.
4. Choose the `main`/`master` branch and `/ (root)` folder, then click **Save**.

### Vercel / Netlify
This is a static site, so it requires zero build configuration. Just drag and drop the folder onto [Netlify](https://www.netlify.com/) or connect the Git repository to [Vercel](https://vercel.com/) for automated CI/CD.

---

## 🧑‍💻 Author

- **Name**: Dipesh Bham
- **Role**: Full Stack Developer, Editor & UI/UX Designer
- **Website**: [dipeshbham.com.np](https://dipeshbham.com.np)
- **LinkedIn**: [Dipesh Bham](https://np.linkedin.com/in/dipesh-bham-b06199378)
- **Instagram**: [@_dipesh.x](https://instagram.com/_dipesh.x)
- **GitHub**: [@dipeshchettry](https://github.com/dipeshchettry)

---

&copy; 2026 Dipesh Bham. Built with passion from Nepal. 🇳🇵
