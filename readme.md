# Zero Space - Sci-Fi Game Website

This is a static website concept for the fictional space exploration and combat game, Zero Space. It's designed with a modern, futuristic aesthetic and built using HTML, Tailwind CSS (via CDN), custom CSS, and vanilla JavaScript. The site is compatible with static hosting platforms like GitHub Pages.

## Features

*   **Futuristic Design:** Dark theme with neon accents, space-themed visuals, and tech-inspired fonts (Orbitron, Exo 2).
*   **Animated Elements:** Includes CSS-animated starfield background, glowing effects, hover transitions, and scroll-triggered fade-in animations.
*   **Responsive Layout:** Adapts to various screen sizes using Tailwind CSS.
*   **Content Sections:** Hero, About, Media (with lightbox), Lore (collapsible panels), Play/Download (with countdown), News, Community.
*   **Interactive Components:** Smooth scrolling, image lightbox, fake "Launch Terminal" modal.
*   **GitHub Pages Ready:** Purely static files (HTML, CSS, JS, assets) with no server-side requirements.

## Tech Stack

*   HTML5
*   CSS3
    *   Tailwind CSS (v3 via CDN)
    *   Custom CSS (`css/styles.css`) for specific animations and effects.
*   JavaScript (Vanilla)
*   Font Awesome (for icons)
*   Google Fonts (Orbitron, Exo 2)

## Project Structure
zero-space-website/
├── index.html # Main HTML file
├── css/
│ └── styles.css # Custom CSS rules and animations
├── js/
│ └── script.js # JavaScript for interactivity (lightbox, scroll, modal, etc.)
├── assets/
│ ├── images/ # Game logo, screenshots, backgrounds
│ └── icons/ # (Optional) SVG icons if not using Font Awesome
└── README.md # This file


## Setup for GitHub Pages

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/yourusername/zero-space-website.git # Replace with your repo URL
    cd zero-space-website
    ```

2.  **Customize Content:**
    *   Replace placeholder text and images in `index.html` with your actual game content.
    *   Update links (social media, download buttons, trailer URL).
    *   Change the game studio name and copyright year in the footer.
    *   Adjust the countdown timer date in `js/script.js`.
    *   Replace placeholder images in `assets/images/`.

3.  **Push to GitHub:**
    *   Create a new repository on GitHub (e.g., `zero-space-website`).
    *   Add the remote origin:
        ```bash
        git remote add origin https://github.com/yourusername/zero-space-website.git
        git branch -M main
        git push -u origin main
        ```
    *   (If you cloned an existing repo, just commit and push your changes):
        ```bash
        git add .
        git commit -m "Initial commit or updates"
        git push origin main
        ```

4.  **Enable GitHub Pages:**
    *   Go to your repository on GitHub.com.
    *   Click on the "Settings" tab.
    *   In the left sidebar, click on "Pages".
    *   Under "Build and deployment", select "Deploy from a branch" as the Source.
    *   Choose the `main` branch (or whichever branch you pushed to).
    *   Keep the folder as `/ (root)`.
    *   Click "Save".

5.  **Access Your Site:** GitHub Pages will build and deploy your site. It might take a minute or two. The URL for your live site (e.g., `https://yourusername.github.io/zero-space-website/`) will be displayed on the Pages settings screen once it's ready.

## Notes

*   **Placeholders:** Remember to replace all placeholder content (images, text, links) with your actual game assets and information.
*   **Tailwind CDN:** This setup uses the Tailwind CSS CDN for simplicity. For production, consider setting up a build process (using Node.js, npm, and the Tailwind CLI) to purge unused styles and optimize the CSS file size.
*   **Performance:** While efforts were made for decent performance (lazy loading via intersection observer), large images or complex animations can still impact load times on static hosting. Optimize assets accordingly.
*   **Discord Widget:** Embedding a live Discord widget directly might be challenging on purely static sites due to security restrictions or JS requirements. The current implementation uses a placeholder and a direct invite link. Research current Discord embedding options if a live widget is crucial.