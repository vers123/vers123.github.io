# Vers123 Game Navigation Website

A clean and beautiful game navigation website providing official navigation links for miHoYo games and other popular games.

![Project Status](https://img.shields.io/badge/Status-Maintained-success)
![License](https://img.shields.io/badge/License-MIT-blue)
![HTML5](https://img.shields.io/badge/HTML5-Latest-orange)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.x-38bdf8)

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Quick Start](#quick-start)
- [Usage](#usage)
- [Tech Stack](#tech-stack)
- [Game List](#game-list)
- [Development Guide](#development-guide)
- [SEO Optimization](#seo-optimization)
- [Performance Optimization](#performance-optimization)
- [FAQ](#faq)
- [Changelog](#changelog)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Project Overview

This project is a static web navigation site that helps users quickly access official websites of various games. It features modern responsive design to provide users with a smooth browsing experience.

### Navigation Categories

- **miHoYo Navigation** - Official website navigation for miHoYo games
- **Another Game Navigation** - Navigation for other popular games

### Project Highlights

- 🎨 **Modern Design** - Built with Tailwind CSS for a beautiful interface
- 📱 **Fully Responsive** - Perfectly adapted for desktop, tablet, and mobile devices
- ⚡ **Fast Loading** - Optimized resource loading for instant access
- 🔍 **SEO Friendly** - Built-in search engine optimization configuration
- 🎯 **User Friendly** - Intuitive navigation structure and interaction design

## Features

### Core Features

- ✅ Responsive design supporting desktop and mobile devices
- ✅ Clean sidebar navigation menu
- ✅ Elegant card layout for game display
- ✅ Click interaction effects (replacing hover effects for better mobile experience)
- ✅ Styled with Tailwind CSS
- ✅ Font Awesome icon library

### Interactive Experience

- 🖱️ Click to switch content areas
- 🎯 Clear game category display
- 🌈 Smooth transition animations
- 📋 Convenient official link navigation

## Project Structure

```
vers123.github.io/
├── index.html                          # Main navigation entry page
├── README.md                           # Project documentation (English)
├── README_CN.md                        # Project documentation (Chinese)
└── Web/
    ├── mihoyo_web/
    │   ├── miHoYo.html                 # miHoYo game navigation page
    │   └── mihoyo/
    │       └── images/
    │           ├── game_logo/          # Game logo images
    │           │   ├── genshin_impact.jpg
    │           │   ├── Honkai Star Rail.jpg
    │           │   ├── zenless_zone_zero.jpg
    │           │   ├── petit_planet.jpg
    │           │   ├── honkai_nexus_anima.jpg
    │           │   ├── honkai_impact_3.jpg
    │           │   ├── tears_of_themis.jpg
    │           │   └── bh2-logo-v2.jpg
    │           └── logo/               # miHoYo logo images
    │               ├── mihoyo.png
    │               ├── mys-logo-v2.png
    │               └── dby-logo-v2.jpg
    └── another_game_web/
        ├── another_games.html          # Other games navigation page
        └── another_games/
            └── images/
                ├── game_logo/          # Game logo images
                │   └── Minecraft.svg
                └── logo/               # Logo images
                    └── Microsoft.png
```

## Quick Start

### Requirements

- Modern browser (Chrome, Firefox, Safari, Edge)
- Internet connection (for loading CDN resources)

### Local Preview

1. **Clone the project**
   ```bash
   git clone https://github.com/vers123/vers123.github.io.git
   cd vers123.github.io
   ```

2. **Open directly**
   - Double-click `index.html` to open in browser
   - Or right-click and select "Open with" > Choose browser

3. **Use local server (optional)**
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js (requires http-server)
   npx http-server -p 8000
   ```
   Then visit `http://localhost:8000` in your browser

### Deploy to GitHub Pages

1. **Push to GitHub**
   ```bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```

2. **Enable GitHub Pages**
   - Go to repository Settings > Pages
   - Source select "Deploy from a branch"
   - Branch select `main` (or `master`)
   - Folder select `/ (root)`
   - Click Save

3. **Access the website**
   - Wait for deployment to complete, then visit `https://yourusername.github.io/vers123.github.io`
   - Or `https://yourusername.github.io/` (if repository name is `yourusername.github.io`)

## Usage

### Navigation Usage

1. **Main Navigation**
   - Open `index.html` to view navigation entry
   - Click corresponding category to enter detailed page

2. **Game Navigation Page**
   - Use left menu to switch game categories
   - Click game cards to visit official websites
   - Browse game introductions and type information

### Custom Configuration

#### Add New Game

Find the game card area in the corresponding HTML file and add a new card:

```html
<a href="Game Official Link" target="_blank" title="Game Name">
  <img src="Image Path" alt="Game Name" class="h-20 md:h-24 lg:h-32 w-auto object-cover">
  <div class="p-4">
    <h3 class="text-xl font-semibold text-gray-800">Game Name</h3>
    <p class="text-gray-600 text-sm mt-1">Game Type Description</p>
  </div>
</a>
```

#### Modify Styles

The project uses Tailwind CSS, you can customize styles by modifying class attributes:

- Colors: `text-gray-800`, `bg-blue-500`, etc.
- Spacing: `p-4`, `m-2`, etc.
- Sizes: `h-20`, `w-auto`, etc.
- Responsive: `md:h-24`, `lg:h-32`, etc.

## Tech Stack

### Frontend Technologies

- **HTML5** - Page structure and semantic tags
- **Tailwind CSS 3.x** - Utility-first CSS framework (via CDN)
- **Font Awesome 4.7** - Icon library (via CDN)
- **JavaScript (ES6+)** - Interactive features and dynamic content switching

### Design Philosophy

- **Mobile First** - Design starting from small screens, progressively adapting to larger screens
- **Progressive Enhancement** - Basic functionality available in all browsers, enhanced features in supporting browsers
- **Performance First** - Minimize resource loading, optimize rendering performance

## Game List

### miHoYo Game Navigation

| Game Name | Type | Official Link |
|-----------|------|---------------|
| Genshin Impact | Open World Adventure | [Official Site](https://genshin.hoyoverse.com) |
| Honkai: Star Rail | Turn-based RPG | [Official Site](https://sr.mihoyo.com/main) |
| Zenless Zone Zero | Action RPG | [Official Site](https://zenless.hoyoverse.com) |
| Petit Planet | Simulation | [Official Site](https://planet.mihoyo.com/home) |
| Honkai: Nexus Anima | Strategy Card | [Official Site](https://yyjl.mihoyo.com/) |
| Honkai Impact 3rd | 3D Action Shooter | [Official Site](https://bh3.mihoyo.com/main) |
| Tears of Themis | Romance Mystery | [Official Site](https://wd.mihoyo.com/main) |
| Guns Girl Z | 2D Action Shooter | [Official Site](https://www.benghuai.com/index/) |

### miHoYo Community Platforms

| Platform Name | Function | Official Link |
|---------------|----------|---------------|
| miHoYo Community | Game Community | [Official Site](https://www.miyoushe.com/) |
| miHoYo Community - Da Bie Shu | Creator Platform | [Official Site](https://www.miyoushe.com/dby) |

### Another Game Navigation

> **Note**: Other popular game navigation pages are under development. Minecraft has been added. More games including League of Legends, Valorant, Apex Legends, Fortnite, Overwatch 2, etc. will be added gradually.

| Game Name | Type | Official Link |
|-----------|------|---------------|
| Minecraft | Sandbox Building | [Official Site](https://www.minecraft.net) |

**Coming Soon Games:**
- League of Legends (MOBA)
- Valorant (Tactical Shooter)
- Apex Legends (Battle Royale)
- Fortnite (Battle Royale)
- Overwatch 2 (Team Shooter)

## Development Guide

### Code Standards

#### HTML Standards

- Use semantic tags (`header`, `nav`, `main`, `footer`)
- All tags must be properly closed
- Images must include `alt` attributes
- When using `target="_blank"` for links, it's recommended to add `rel="noopener noreferrer"`

#### CSS Standards

- Prioritize Tailwind CSS utility classes
- Custom styles should be placed in `<style>` tags
- Keep class names concise and clear
- Follow mobile-first principles

#### JavaScript Standards

- Use `const` and `let` instead of `var`
- Use arrow functions or traditional function declarations
- Use `addEventListener` or inline events for event handling
- Keep code concise, avoid redundant logic

### Debugging Tips

1. **Browser Developer Tools**
   - Press F12 to open developer tools
   - Use Elements panel to check HTML and CSS
   - Use Console panel to view JavaScript errors
   - Use Network panel to check resource loading

2. **Responsive Testing**
   - Use device simulation mode in developer tools
   - Test different screen sizes (320px, 768px, 1024px, 1920px)
   - Check display on mobile and desktop

3. **Performance Testing**
   - Use Lighthouse for performance scoring
   - Check resource loading times
   - Optimize image sizes and formats

## SEO Optimization

### Implemented Optimizations

- ✅ Meta description tags
- ✅ Meta keywords tags
- ✅ Author information tags
- ✅ Semantic HTML structure
- ✅ Image alt attributes
- ✅ Friendly URL structure

### Meta Tag Example

```html
<meta name="description" content="Vers123 Game Navigation Website - Providing official navigation links for miHoYo games and other popular games">
<meta name="keywords" content="game navigation,miHoYo,Genshin Impact,Honkai Star Rail,game official site,game links">
<meta name="author" content="Vers123">
```

### SEO Recommendations

1. **Regular Content Updates** - Keep game information up-to-date
2. **Image Optimization** - Use appropriate file formats and compression
3. **Improve Loading Speed** - Optimize resource loading order
4. **Build Backlinks** - Increase external links to the website
5. **Submit to Search Engines** - Submit website to Google, Baidu, etc.

## Performance Optimization

### Implemented Optimizations

- ✅ CDN loading for external resources
- ✅ Responsive images
- ✅ Minimized JavaScript
- ✅ CSS utility classes priority
- ✅ Avoid unnecessary DOM operations

### Performance Metrics

- **First Contentful Paint (FCP)**: < 1.5s
- **Largest Contentful Paint (LCP)**: < 2.5s
- **First Input Delay (FID)**: < 100ms
- **Cumulative Layout Shift (CLS)**: < 0.1

### Optimization Recommendations

1. **Image Optimization**
   - Use WebP format
   - Compress image sizes
   - Use lazy loading (`loading="lazy"`)

2. **Code Optimization**
   - Minify HTML, CSS, JavaScript
   - Remove unused code
   - Use code splitting

3. **Caching Strategy**
   - Set appropriate cache headers
   - Use Service Worker
   - Leverage browser caching

## FAQ

### Q: Why are some images not displaying?

A: Please check the following:
- Confirm image paths are correct
- Check if image files exist
- Confirm image formats are supported
- Check if network connection is normal

### Q: How do I add new games?

A: Follow these steps:
1. Prepare game logo images and place them in the corresponding `game_logo` folder
2. Find the game card area in the HTML file
3. Copy existing card code
4. Modify links, image paths, game names, and descriptions

### Q: How do I modify website theme colors?

A: Tailwind CSS uses class names to control styles, you can:
1. Modify color class names (e.g., change `text-blue-500` to `text-red-500`)
2. Add custom styles in `<style>` tags
3. Use CSS variables for theme switching

### Q: Which browsers does the website support?

A: This website supports the following modern browsers:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

IE browser is not supported.

### Q: How to get the best experience on mobile devices?

A: Recommendations:
- Use Chrome or Safari browser
- Ensure stable network connection
- Landscape browsing provides better display

## Changelog

### v2.1 (2025-12-23)

- 🌐 Added English version of website (miHoYo_EN.html, another_games_EN.html)
- 📝 Renamed original README.md to README_CN.md
- ✅ Created new README.md as language selection entry page
- ✅ Updated index.html with Chinese and English version links
- ✅ Enhanced project documentation with bilingual support

### v2.0 (2025-12-23)

- 🚀 Major project update
- ✨ Added Minecraft game content to Another Game navigation page
- ✨ Added Minecraft and Microsoft logo image resources
- ✨ Updated README.md to reflect Minecraft addition
- ✅ Completed comprehensive project check and verification
- ✅ All page functions normal, image resources complete

### v1.0 (2025-12-23)

- 🎉 Initial project release
- ✨ Created main navigation entry page
- ✨ Implemented miHoYo game navigation page
- ✨ Implemented Another Game navigation page
- ✨ Implemented responsive design supporting desktop and mobile devices
- ✨ Added Font Awesome icons
- ✨ Built beautiful interface with Tailwind CSS
- ✨ Added sidebar navigation menu
- ✨ Implemented click-to-switch content area interaction
- ✨ Added SEO optimization (meta tags)
- ✨ Created detailed README documentation
- ✅ Completed project verification and testing

---

<div align="center">

**If this project helps you, please give it a ⭐️**

Made with ❤️ by Vers123

© 2025 Vers123 | This website is for demonstration purposes only

</div>
