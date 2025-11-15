# 🚀 Raman Kumar Sha | Personal Portfolio Website

A clean, responsive, and modern personal portfolio showcasing skills, professional journey, and projects as a **Frontend Developer**.

## ✨ Features

This portfolio is designed to be highly engaging and user-friendly, providing a comprehensive overview of the developer's profile and work.

* **Responsive Design:** Fully adapts to mobile, tablet, and desktop screens using modern CSS techniques.
* **Hero Section:** Prominent welcome area with a brief introduction, professional photo card, and key calls-to-action (Contact Me, Download Resume).
* **Interactive Menu:** A clean, fixed navigation menu with a smooth overlay for quick access to different sections.
* **Animated Skills:** Visually engaging display of technical skills using subtle animations and popular dev icons (HTML, CSS, JavaScript, React, etc.).
* **Timeline/Journey:** A structured, fading-in timeline to narrate the educational and professional path.
* **Projects Slider:** A dedicated section with a horizontal carousel/slider for showcasing key projects.
* **Connect Section:** A visually appealing contact section with social media links and a gradient wave design.
* **Pure HTML, CSS, and JavaScript:** Built without external libraries or frameworks for maximum performance and a deep understanding of core web technologies.

## 🛠️ Tech Stack

This project leverages the fundamental pillars of web development for a fast and lightweight experience.

| Category | Technology | Description |
| :--- | :--- | :--- |
| **Structure** | `HTML5` | Semantic and accessible markup for the entire page content. |
| **Styling** | `CSS3` | Custom styling with `flexbox`, `grid`, `keyframes`, and `gradients` for complex layouts and animations. |
| **Interactivity** | `JavaScript (Vanilla)` | Used for the menu toggle, project slider functionality, scroll-based animations, and CTA handling. |
| **Icons** | `Devicons` / `Font Awesome` | Used for skill icons and social media branding. |
| **Fonts** | `Google Fonts` | Inter, Playfair Display, and Poppins for modern typography. |

---

## 📂 Project Structure

The entire portfolio is contained within a single `index.html` file, which includes all the CSS (in `<style>` tags) and JavaScript (in `<script>` tags).

### Key HTML Sections

The portfolio is logically divided into sections, each with a specific `id` for navigation:

1.  **`<header id="hero-section">`:**
    * Contains the main title, short description, and the profile card.
    * Includes the fixed brand name and the hamburger menu button/overlay.
2.  **`<section id="skills-section">`:**
    * Displays the core competency text and floating skill icon lists.
3.  **`<section id="journey-section">`:**
    * The vertical timeline detailing the developer's education and career milestones.
4.  **`<section id="projects-section">`:**
    * Houses the horizontal project carousel/slider.
5.  **`<section id="connect-section">`:**
    * The footer-like section for social media connections and contact information, featuring the SVG wave background.

### Key CSS Features (`<style>`)

* **Hero Animation:** The `::before` pseudo-element uses a `repeating-linear-gradient` with the `@keyframes heroShine` to create a subtle, moving background pattern.
* **Responsive Grid:** Media queries (`@media (max-width:980px)`) are used to switch the `#hero-inner` from a two-column grid to a single column stack.
* **Card Hover Effect:** The `.profile-card:hover` selector applies a `transform: translateY(-6px);` for a subtle lift effect.
* **Timeline Fade:** The `.fade` and `.fade.show` classes work with JavaScript to create a staggered, scroll-reveal animation for the journey items.

### Key JavaScript Functionality (`<script>`)

1.  **Navigation (`menuBtn`/`menuOverlay`):**
    * Handles the opening and closing of the full-screen menu overlay using `classList.toggle('active')`.
    * Includes an **Escape key listener** for accessibility and quick closing.
2.  **CTA/Resume (`downloadResume`):**
    * Attaches a click listener to the "Download Resume" button to dynamically create an `<a>` tag and trigger the download of the local resume file (`assets/Raman_Kumar_Resume.pdf`).
3.  **Scroll Reveal (`reveal` function):**
    * Uses `window.addEventListener("scroll", reveal)` and `getBoundingClientRect().top` to check when a timeline item enters the viewport, adding the `.show` class for the fade-in animation.
4.  **Projects Slider:**
    * Manages the `position` variable to calculate the necessary `translateX` value.
    * The `next` and `prev` buttons update the `position` based on the calculated `cardWidth` and the number of cards visible in the current viewport.

---

## ⚙️ Setup and Usage

To run this portfolio locally:

1.  **Clone the repository:**
    ```bash
    git clone [Your Repository URL]
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd [project-folder-name]
    ```
3.  **Open the file:**
    Simply open the `index.html` file in your web browser.

**Note:** Ensure you replace the placeholder image paths and links with your actual content:

* Update the `src` for the profile image in the `<div class="profile-card">`.
* Update the `href` for the social media links in the `<section id="connect-section">`.
* Place your resume PDF at the path specified in the JavaScript: `assets/Raman_Kumar_Resume.pdf`.

---

## ✍️ Author

**Raman Kumar Sha**
* **Role:** Frontend Developer
* **Contact:** [kumaraman57y@gmail.com](mailto:kumaraman57y@gmail.com)
* **LinkedIn:** [https://www.linkedin.com/in/raman-kumar-948111342/](https://www.linkedin.com/in/raman-kumar-948111342/)
* **GitHub:** [https://github.com/kumaraman57y](https://github.com/kumaraman57y)

***

Designed and Developed with ❤️ by Raman.