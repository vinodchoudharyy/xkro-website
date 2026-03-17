# Xkro Solution Private Limited - Company Website

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Static Site](https://img.shields.io/badge/Static-HTML/CSS/JS-brightgreen.svg)](https://xkro.in)

## 🚀 Quick Start

1. Clone/Download the repo
2. Open `index.html` in any modern browser (Chrome/Firefox/Safari recommended)
3. No server or build tools required!

Live Demo: [View Website](index.html) | Live Project: [https://xkro.in](https://xkro.in)

## 📱 Features

- **Single Page Application (SPA)**: Smooth navigation between Company, App, Services, Hire Us, Contact
- **Modern Glassmorphism Design**: Backdrop blur navbar, gradient accents, floating particles
- **Dark Mode**: Toggle with moon/sun button (persists via localStorage)
- **Animations**: Scroll-reveal, floating logo, pulse glow, count-up stats, hero particles
- **Interactive Elements**:
  - Collapsible accordions (Hire Us/FAQ)
  - EmailJS contact form (no backend needed)
  - Custom cursor (desktop only)
  - Floating WhatsApp/Call buttons
  - Sticky scroll-to-top
- **Responsive**: Mobile-first design (breakpoints: 860px tablet, 640px mobile, 420px extra-small)
- **Performance**: Inline CSS/JS for instant load, optimized animations
- **3D Hero**: Vanta.js Globe effect (Three.js powered)

## 🛠 Tech Stack

| Category | Technologies |
|----------|--------------|
| **Frontend** | HTML5, CSS3 (Grid/Flexbox/CSS Vars/Animations), Vanilla JavaScript |
| **Icons/Fonts** | Font Awesome 6, Google Fonts (Montserrat, Open Sans) |
| **Effects** | Vanta.js Globe + Three.js |
| **Form** | EmailJS (service_xkro, template_xkro - configure your public key) |
| **Images** | Unsplash (hero/service banners), logo.png (local) |
| **External** | Play Store QR/app links, Google Maps iframe |

## 📂 Project Structure

```
xkro-website/
├── index.html      # Main SPA (all pages/sections)
├── logo.png        # Company logo (nav/hero/preloader)
└── README.md       # You're reading it!
```

## 🎨 Sections Breakdown

1. **Hero**: Animated globe, stats counter (50+ projects, 30+ clients etc.)
2. **About**: Mission/Vision cards
3. **How We Work**: 4 pricing/work models (Fixed Rate, Time Base, Dedicated, Revenue Share)
4. **Xkro Works**: Escrow transaction flow (2 options)
5. **Features & Safety**: 7 security highlights
6. **FAQ**: 5 expandable questions
7. **App Promo**: Download cards + QR for Android/iOS
8. **Services/Hire**: Cards/accordions for dev services
9. **Contact**: Form + info blocks + Google Maps

**Page Variants**: App/Services/Hire/Contact reuse footer + app promo with unique banners.

## ⚙️ Customization Guide

### Update Contact/Branding
```html
<!-- EmailJS: Replace 'YOUR_EMAILJS_PUBLIC_KEY' in script -->
emailjs.init('YOUR_PUBLIC_KEY');

<!-- Phone/Email/Address in HTML -->
<a href="tel:+918107093963">+91 8107093963</a>
<a href="mailto:Support@xkro.in">Support@xkro.in</a>
```

### Play Store Link
```html
<a href="https://play.google.com/store/apps/details?id=com.xkro.app">Google Play</a>
```

### Logo
Replace `logo.png` (42x42px recommended, PNG transparent).

### Colors/Theme
Edit CSS `:root` vars:
```css
--teal: #4ab8d4;
--accent: #6c63ff;
--magenta: #ff6b9d;
```

### EmailJS Setup
1. [EmailJS Dashboard](https://dashboard.emailjs.com)
2. Add service `service_xkro`, template `template_xkro`
3. Replace init key in `index.html`

## 🔍 Development Notes

### Code Organization
- **Inline Styles/Scripts**: ~2000+ lines for zero-dependency. Consider splitting for larger projects.
- **Key Functions**:
  ```js
  go(page)     // SPA navigation
  toggleH/Faq  // Accordions
  submitForm() // EmailJS
  initReveal() // Scroll animations
  ```
- **Animations**: IntersectionObserver for reveals, requestAnimationFrame for counters.
- **Responsive**: `@media` queries cascade perfectly.

### Performance Tips
- Minify inline CSS/JS for production
- Lazy-load images if adding more
- Vanta.js: Disable on mobile if needed (`gyroControls: false`)

### Browser Support
- Chrome 80+, Firefox 75+, Safari 13.1+, Edge 80+
- Custom cursor disabled on touch/mobile

## 📸 Screenshots

![Hero Section](https://via.placeholder.com/1200x600/0f172a/ffffff?text=Hero+Globe)
![Services](https://via.placeholder.com/1200x400/ffffff/2c2c2c?text=Services+Cards)
![Dark Mode](https://via.placeholder.com/1200x600/16213e/e0e8f5?text=Dark+Mode)

*(Replace with actual screenshots)*

## 🚀 Deployment

```bash
# GitHub Pages/Netlify/Vercel: Drag/drop index.html + logo.png
# Or serve static folder
npx serve .
```

## 🤝 Contributing

1. Fork repo
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit (`git commit -m 'Add some AmazingFeature'`)
4. Push (`git push origin feature/AmazingFeature`)
5. Open Pull Request

## 📄 License

This project is [MIT](LICENSE) licensed.

## 🙌 Acknowledgments

- [Vanta.js](https://www.vantajs.com/) - 3D effects
- [EmailJS](https://www.emailjs.com/) - Contact forms
- [Unsplash](https://unsplash.com/) - Hero images

---

**⭐ Star the repo if helpful!**  
**Contact**: [support@xkro.in](mailto:support@xkro.in) | [+91 8107093963](tel:+918107093963)
