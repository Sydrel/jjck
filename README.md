# JJCK Collectibles - Premium Sports Cards & Collectibles Website

A modern, responsive single-page website for JJCK Collectibles, a family-owned sports card and collectibles shop located in Port St. Lucie, Florida.

## 📋 Overview

This is a complete HTML/CSS/JavaScript website designed for JJCK Collectibles, featuring a full-screen hero slideshow, business hours display, event promotions, brand showcases, and a contact modal. The site is fully responsive and optimized for all devices from desktop to mobile.

## ✨ Features

- **Full-Screen Hero Slideshow** - Auto-playing image carousel with manual navigation controls
- **Dynamic Business Hours** - Real-time open/closed status with color-coded indicators
- **Contact Modal** - Easy access to store information, hours, and directions
- **Responsive Design** - Optimized for desktop, tablet, and mobile devices
- **Social Media Integration** - Links to Facebook, Instagram, TikTok, YouTube, Yelp, and Discord
- **Event Promotion** - Featured events section with ticket links
- **Brand Showcase** - Clickable brand logos linking to shop categories
- **Promotional Banner** - WhatNot auction integration and Facebook giveaway promotion
- **Mobile-First Navigation** - Hamburger menu for smaller screens

## 🛠️ Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Custom properties, flexbox, grid, media queries
- **JavaScript (Vanilla)** - Slideshow, modal, hours tracking, navigation
- **Google Fonts** - Oswald (headings) & Roboto (body)
- **Font Awesome** - Icon library
- **GitHub Pages** - Hosting (recommended)

## 📁 Project Structure

```
jjck-collectibles/
├── index.html          # Main HTML file (contains all CSS & JS)
├── README.md           # Project documentation
└── assets/            # (Optional) Images and other assets
```

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Basic text editor for modifications (VS Code, Sublime Text, etc.)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/jjck-collectibles.git
   ```

2. **Navigate to the project directory:**
   ```bash
   cd jjck-collectibles
   ```

3. **Open the website:**
   - Double-click `index.html` in your file explorer, OR
   - Use a local development server:
     ```bash
     # Using Python 3
     python -m http.server 8000
     
     # Using Node.js (with live-server)
     npx live-server
     ```

4. **View in browser:**
   Open `http://localhost:8000` (or the port you specified)

## 🎨 Customization

### Updating Business Hours

The business hours are defined in the JavaScript `updateHoursStatus()` function:

```javascript
const dayHours = {
    0: { open: 12, close: 16 }, // Sunday
    1: { open: 10, close: 18 }, // Monday
    2: { open: 10, close: 18 }, // Tuesday
    3: { open: 10, close: 18 }, // Wednesday
    4: { open: 10, close: 18 }, // Thursday
    5: { open: 10, close: 18 }, // Friday
    6: { open: 10, close: 18 }  // Saturday
};
```

**Hours format:** 24-hour time (0-23)  
**Example:** `{ open: 9, close: 17 }` = 9:00 AM - 5:00 PM

### Updating Hero Slideshow Images

The hero slideshow images are set in the CSS:

```css
.hero-slide:nth-child(1) {
    background-image: url('//img1.wsimg.com/...');
}
.hero-slide:nth-child(2) {
    background-image: url('https://i.imgur.com/4nEycte.jpeg');
}
/* ... continue for all slides */
```

To add or remove slides:
1. Update the CSS background images
2. Update the HTML dots in the `.hero-dots` section
3. Update the JavaScript `heroSlides` selection if needed

### Updating Social Media Links

Social media links appear in three places:
1. **Social Strip** (below hero)
2. **Footer Community section**
3. **Footer Social icons**

Update the URLs in the `<a href="...">` tags for each platform:

```html
<a href="https://www.facebook.com/jjckcollectibles" target="_blank">
    <i class="fab fa-facebook-f"></i>
</a>
```

### Adding/Removing Brand Logos

The brand logos section is in the HTML:

```html
<div class="brand-logo-card">
    <a href="https://www.jjckcollectibles.com/shop/magic" target="_blank">
        <img src="https://example.com/logo.png" alt="Brand Name">
    </a>
</div>
```

Each card should include:
- An `<a>` tag with the shop URL
- An `<img>` tag with the logo image URL
- Appropriate `alt` text for accessibility

### Changing Colors

The color scheme is controlled by CSS variables in the `:root` selector:

```css
:root {
    --bg-dark: #000000;
    --text-primary: #ffffff;
    --text-secondary: #bbbbbb;
    --text-muted: #777777;
    --yellow: #FFFF33;
    --green: #4ade80;
    --red: #ef4444;
    /* ... */
}
```

## 📱 Responsive Breakpoints

- **Desktop**: > 1024px - Full layout
- **Tablet**: 768px - 1024px - Adjusted spacing, centered content
- **Mobile**: 480px - 768px - Stacked layout, smaller fonts
- **Small Mobile**: < 480px - Compact layout, minimal spacing

## 🔧 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Opera (latest)
- Mobile browsers (iOS Safari, Android Chrome)

## 📝 SEO & Accessibility

- Semantic HTML5 elements
- ARIA labels for interactive elements
- Alt text for images
- Proper heading hierarchy
- Meta description for search engines
- Open Graph tags for social sharing (can be added)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is proprietary and owned by JJCK Collectible's LLC. All rights reserved.

## 📧 Contact

- **Website**: [jjckcollectibles.com](https://jjckcollectibles.com)
- **Email**: jjckcollectibles@gmail.com
- **Phone**: 1-772-249-5036
- **Address**: 1344 SW Bayshore Blvd, Port St. Lucie, FL 34983

## 🌐 Social Media

- [Facebook](https://www.facebook.com/jjckcollectibles)
- [Instagram](https://www.instagram.com/jjckcollectibles/)
- [TikTok](https://www.tiktok.com/@jjckcollectibles)
- [YouTube](https://www.youtube.com/@JJCKCollectibles)
- [Yelp](https://www.yelp.com/biz/jjck-collectibles-port-st-lucie)
- [Discord](https://discord.com/invite/WmpvsK8Uhx)

---

**JJCK Collectibles** - Where Collectors Become Family 🃏
