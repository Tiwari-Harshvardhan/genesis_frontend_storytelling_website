# Genesis: The Chronology of Life

An interactive, immersive web experience exploring 3.8 billion years of evolutionary history — from primordial chemistry to human consciousness.

## 🌍 Overview

**Genesis: The Chronology of Life** is a beautifully designed, single-page application that takes you on a visual journey through Earth's biological history. Using cutting-edge web technologies and stunning animations, it tells the story of how life emerged, evolved, and eventually became aware of itself.

### Five Epic Chapters

1. **The Primal Soup** — The first self-replicating molecules 3.8 billion years ago
2. **The Deep Blue** — The Cambrian Explosion and the birth of complex life
3. **The Great Migration** — When creatures first ventured onto land
4. **Age of Giants** — 165 million years of dinosaur dominance
5. **The Human Dawn** — From apes to consciousness in just 7 million years

## 🎨 Features

- **Interactive Animations**: Smooth scroll-triggered animations powered by GSAP and ScrollTrigger
- **3D Background**: Dynamic star field and floating bioluminescent orbs rendered with Three.js
- **Particle Effects**: Real-time 2D particle animations on the Primal Soup chapter
- **Custom Cursor**: Smooth, glowing cursor that responds to interactions
- **Timeline Navigation**: Right-side dot navigation system for quick chapter access
- **Modal Details**: Click era cards to explore detailed information and statistics
- **Parallax Effects**: Multi-layer landscape parallax on the Great Migration section
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Loading Screen**: Immersive loading sequence with DNA animation

## 🚀 Getting Started

### Quick Start

1. **Download or Clone** the repository:
   ```bash
   git clone https://github.com/yourusername/genesis-chronology.git
   cd genesis-chronology
   ```

2. **Open in Browser**:
   - Simply double-click `genesis-chronology.html` or open it in your browser
   - No build process or server required!

3. **Live Server (Recommended)**:
   ```bash
   # Using VS Code Live Server extension or Python's built-in server
   python -m http.server 8000
   # Then visit http://localhost:8000
   ```

## 📋 Requirements

- **Browser**: Modern browser with WebGL and ES6 support (Chrome, Firefox, Safari, Edge)
- **Internet Connection**: Required for CDN resources (fonts, libraries)
- **No Dependencies to Install**: All libraries are loaded from CDN

### External Dependencies

The project uses the following libraries loaded from CDN:

- **GSAP 3.12.5** — Advanced animation library with ScrollTrigger plugin
- **Three.js r128** — 3D graphics library for WebGL rendering
- **Google Fonts** — Cormorant Garamond and Space Mono typefaces

## 🎯 How to Use

### Navigation

- **Scroll** through the entire experience
- **Click chapter links** in the top navigation or timeline dots on the right
- **Hover** on era cards to reveal more information
- **Click era cards** to open detailed modal with statistics
- **Move your mouse** on the Primal Soup section to interact with particles

### Timeline Sidebar

The timeline dots on the right side of the screen allow you to:
- Jump to any chapter instantly
- See which chapter you're currently viewing (highlighted dot)
- Hover to see chapter names

### Progress Bar

The thin gradient bar at the very top shows your progress through the entire experience.

## 📁 File Structure

```
genesis-chronology.html          # Main application (single file)
README.md                         # This file
.gitignore                        # Git configuration
```

## 🛠️ Customization Guide

### Modifying Content

All content is embedded in the HTML file. To edit:

1. **Chapter Text**: Search for `<p class="chapter-body">` and modify the text
2. **Chapter Titles**: Search for `<h2 class="chapter-title">` to change titles
3. **Era Cards**: Look for `data-title`, `data-body` attributes in the XML to update card information
4. **Evolution Timeline**: Modify the `.evo-step` divs in Chapter 5

### Styling

All CSS is contained within the `<style>` tags:

- **Color Variables**: Defined in `:root` pseudo-class — modify `--biolum`, `--amber`, etc.
- **Typography**: Font family and sizes are CSS custom properties for easy adjustment
- **Layout**: Grid and flexbox systems respond to viewport size with clamp() functions

### Animations

GSAP animations are configured in the JavaScript section:

- **Scroll Triggers**: Modify trigger points with `start` and `end` properties
- **Timing**: Change `duration` values to speed up/slow down animations
- **Easing**: Experiment with different GSAP easing functions (`.out`, `.in`, etc.)

### Three.js Scene

The 3D background can be customized by modifying:

- **Star Count**: Change `const starCount = 800;` to increase/decrease stars
- **Orb Count**: Modify the `for (let i = 0; i < 30; i++)` loop count
- **Colors**: Update `orbColors` array with hex values

## ⚙️ Performance Tips

- For lower-end devices, reduce particle count and orb count in JavaScript
- Disable Three.js effects if experiencing lag with `renderer.render(scene, camera);`
- Consider reducing animation complexity on mobile devices

## 🌐 Deployment

Deploy easily to any static hosting service:

- **GitHub Pages**: Push to `gh-pages` branch
- **Vercel**: Connect your repository for automatic deployments
- **Netlify**: Drag-and-drop the file or connect your repo
- **Traditional Hosting**: Upload `genesis-chronology.html` to any web server

## 🎓 Educational Use

This project is perfect for:

- Biology and evolution education
- Science visualization demonstrations
- Portfolio showcase for web developers
- Interactive storytelling examples
- Animation and design inspiration

## 🔧 Troubleshooting

### Animations Are Choppy

- Reduce background orb count from 30 to 15
- Disable particle interactions on Ch1
- Lower particle count from 120 to 60

### 3D Background Not Rendering

- Ensure WebGL is enabled in your browser
- Update your graphics drivers
- Try a different browser

### Fonts Not Loading

- Check your internet connection (fonts load from Google Fonts)
- Clear browser cache and reload

### Mobile Display Issues

- Zoom is intentionally disabled for best experience
- All elements should be readable and interactive
- Test in landscape mode for better viewing

## 💡 Browser Support

| Browser | Support | Notes |
|---------|---------|-------|
| Chrome | ✅ Full | Recommended |
| Firefox | ✅ Full | Excellent performance |
| Safari | ✅ Full | Tested on macOS/iOS |
| Edge | ✅ Full | Chromium-based |
| IE 11 | ❌ No | Use modern browser |

## 📝 Credits & Attribution

Inspired by scientific documentaries and the wonder of evolutionary biology. Special thanks to:

- Carl Sagan (featured quote)
- GSAP and ScrollTrigger teams
- Three.js community

## 📄 License

This project is open source. Feel free to use, modify, and share!

## 🤝 Contributing

Found a bug or have suggestions?

1. Fork the repository
2. Create a feature branch
3. Make your improvements
4. Submit a pull request

## 📧 Contact

Have questions or feedback? Feel free to reach out!

---

**Made with ❤️ and a lot of JavaScript**

*"We are a way for the cosmos to know itself." — Carl Sagan*
