# Birthday Celebration Website

A beautiful, interactive birthday website featuring animated hearts, blooming flowers, and personalized messages. Built with modern JavaScript (ES6+) and HTML5 Canvas animations.

## Features

- **Animated Heart Shape**: Canvas-based heart animation with blooming flower effects
- **Real-time Counter**: Live time elapsed since birthday with beautiful digital font
- **Interactive Elements**: Smooth fade-in animations and typewriter effects
- **Responsive Design**: Works across different screen sizes
- **Modern Code**: Built with ES6+ classes and vanilla JavaScript (no dependencies)
- **Personal Touch**: Customizable messages and Shakespeare quotes

## Preview

<img src="https://raw.githubusercontent.com/rkruk/bday.website/master/bday.png" alt="Birthday Website Preview">

**Live Demo**: [View the website in action](https://rkruk.github.io/bday.website)

## Project Structure

```
bday.website/
├── index.html          # Main HTML file with birthday message template
├── bday.png           # Preview screenshot
├── digital-7_mono.ttf # Digital font for time counter
├── css/
│   └── default.css    # Styling for layout, fonts, and animations
├── js/
│   ├── garden.js      # Canvas animation engine (flowers, particles)
│   ├── birthday-app.js # Main application logic and heart animation
│   ├── functions_dev.js # Development utilities (legacy)
│   ├── garden_dev.js   # Development version (legacy)
│   └── jquery.js      # jQuery library (legacy, not used in modern version)
└── README.md          # This file
```

## Getting Started

### Quick Start

1. **Clone the repository**:
   ```bash
   git clone https://github.com/rkruk/bday.website.git
   cd bday.website
   ```

2. **Open in browser**:
   - Simply open `index.html` in your web browser
   - Or use a local server for better experience:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js (if you have live-server installed)
   npx live-server
   ```

3. **View the website**:
   - Navigate to `http://localhost:8000` (if using server)
   - Or directly open the `index.html` file

### Customization

To personalize the birthday message:

1. **Edit the HTML content** in `index.html`:
   - Replace `(add_Birthday_Person_Name)` with the person's name
   - Update `(add_day_here)` and `(add_month_here)` with birthday details
   - Modify the date in the code section

2. **Customize styling** in `css/default.css`:
   - Change colors, fonts, or layout
   - Adjust animation timings

3. **Modify messages** in the HTML:
   - Update the Shakespeare quotes
   - Change the birthday wishes

## Technical Details

### Modern JavaScript Architecture

The project uses modern ES6+ features:

- **Classes**: `BirthdayApp` and `Garden` classes for clean organization
- **Modules**: Modern module structure (can be easily converted to ES modules)
- **Canvas API**: HTML5 Canvas for smooth animations
- **Modern DOM**: Uses vanilla JavaScript instead of jQuery
- **Performance**: Optimized with `requestAnimationFrame` for smooth animations

### Key Components

1. **BirthdayApp Class** (`js/birthday-app.js`):
   - Main application controller
   - Handles heart animation sequence
   - Manages time counter and message display
   - Provides smooth fade-in and typewriter effects

2. **Garden Class** (`js/garden.js`):
   - Canvas animation engine
   - Creates and manages flower particles
   - Handles bloom effects and particle physics
   - Renders the animated background

3. **Styling** (`css/default.css`):
   - Responsive layout system
   - Digital font integration
   - Animation definitions
   - Color scheme and typography

### Animation Flow

1. **Initialization**: Canvas setup and garden preparation
2. **Heart Drawing**: Animated heart shape drawn point by point
3. **Flower Blooming**: Particles bloom at each heart point
4. **Message Display**: Fade-in effects for birthday messages
5. **Time Counter**: Real-time elapsed time since birthday

## Customization Guide

### Changing Colors

Edit `css/default.css` to modify the color scheme:

```css
/* Main background */
body { background: #000; }

/* Text colors */
.comments { color: #7F7F7F; }
.keyword { color: #06C; }
.string { color: #080; }
```

### Modifying Animation Speed

Adjust timing in `js/birthday-app.js`:

```javascript
// Heart animation speed (lower = faster)
const interval = 5;

// Fade-in duration (milliseconds)
this.fadeIn(element, 3000);
```

### Adding Custom Messages

Update the HTML in `index.html`:

```html
<div id="messages">
    <div id="loveu">
        Your custom birthday message here!
    </div>
</div>
```

## Development

### File Purposes

- **`index.html`**: Main page with birthday message template
- **`js/birthday-app.js`**: Core application logic (modern ES6+)
- **`js/garden.js`**: Animation engine for particles and effects
- **`css/default.css`**: All styling and layout rules
- **`digital-7_mono.ttf`**: Digital font for the time counter

## Browser Compatibility

- **Modern Browsers**: Chrome, Firefox, Safari, Edge (latest versions)
- **Features Used**: HTML5 Canvas, ES6+ JavaScript, CSS3 animations
- **Mobile**: Responsive design works on mobile devices

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).

## Credits

- **Original Concept**: Birthday celebration with code and flowers
- **Modernization**: Updated to ES6+ and modern web standards (2025)
- **Inspiration**: Shakespeare quotes and romantic poetry
- **Font**: Digital-7 Mono for retro digital clock effect

---

*Made with ❤️ for special birthday celebrations*
