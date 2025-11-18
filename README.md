# Modern Portfolio Website

A modern, minimal Portflow-style portfolio website for developers and designers. Built with clean aesthetics, large typography, smooth scroll animations, and a grid-based layout.

## 🎨 Features

- **Modern Design**: Clean white background with black/gray accents
- **Smooth Animations**: Scroll-triggered animations and parallax effects
- **Responsive Layout**: Fully responsive design for all devices
- **Fast Loading**: Optimized for performance
- **Two Versions**: 
  - HTML/CSS/JavaScript version
  - React + Tailwind CSS version

## 📁 Project Structure

```
port/
├── index.html          # Main HTML file
├── css/
│   └── style.css      # All styles and animations
├── js/
│   └── script.js      # JavaScript for interactions
├── images/
│   └── rohith.jpg     # Profile image
├── react-portfolio/   # React + Tailwind version
│   ├── src/
│   │   ├── components/
│   │   │   ├── Navbar.jsx
│   │   │   ├── Hero.jsx
│   │   │   ├── About.jsx
│   │   │   ├── Skills.jsx
│   │   │   ├── Projects.jsx
│   │   │   ├── Experience.jsx
│   │   │   ├── Testimonials.jsx
│   │   │   ├── Contact.jsx
│   │   │   └── Footer.jsx
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   └── index.css
│   ├── package.json
│   └── vite.config.js
└── README.md
```

## 🚀 Quick Start

### HTML/CSS Version

Simply open `index.html` in your browser or use a local server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve .
```

Then open `http://localhost:8000` in your browser.

### React + Tailwind Version

1. Navigate to the React portfolio directory:
```bash
cd react-portfolio
```

2. Install dependencies:
```bash
npm install
```

3. Run the development server:
```bash
npm run dev
```

4. Build for production:
```bash
npm run build
```

5. Preview production build:
```bash
npm run preview
```

## 📋 Sections

1. **Hero Banner** - Name, title, and introduction
2. **About Me** - Personal story and statistics
3. **Skills** - Technical skills with progress bars
4. **Projects** - Featured projects gallery (3 different types)
5. **Experience** - Timeline of work experience
6. **Testimonials** - Client testimonials
7. **Contact** - Contact form and information

## 🎨 Design Specifications

### Colors
- Primary: `#000000` (Black)
- Secondary: `#333333` (Dark Gray)
- Accent: `#666666` (Medium Gray)
- Background: `#FFFFFF` (White)
- Light Background: `#F8F8F8` (Off-White)

### Typography
- Font Family: Inter (Google Fonts)
- Font Weights: 300, 400, 500, 600, 700, 800
- Large typography for headings (clamp for responsiveness)

### Spacing & Layout
- Container max-width: 1200px
- Section padding: 6rem vertical
- Grid-based layout with gap spacing
- Rounded corners: 8px - 16px
- Soft shadows: `0 4px 20px rgba(0, 0, 0, 0.08)`

### Animations
- Smooth scroll behavior
- Fade-in animations on scroll
- Parallax effects for images
- Hover transitions (300ms cubic-bezier)
- Skill bar progress animations
- Counter animations for statistics

## 📱 Responsive Breakpoints

- Mobile: < 768px
- Tablet: 768px - 968px
- Desktop: > 968px

## 🔧 Customization

### Update Personal Information

1. **Hero Section**: Edit name and title in `index.html` or `Hero.jsx`
2. **About Section**: Update the about text
3. **Projects**: Modify project details in the projects section
4. **Experience**: Update timeline entries
5. **Contact**: Change contact information

### Change Colors

Edit CSS variables in `css/style.css`:
```css
:root {
    --primary-color: #000000;
    --secondary-color: #333333;
    /* ... */
}
```

Or update Tailwind config in `react-portfolio/tailwind.config.js`

### Add/Remove Projects

Currently showing 3 different types of projects:
1. Real-Time Object Detection (AI/Computer Vision)
2. Weather Application (Web Development)
3. AI Trend Forecast App (Data Science/ML)

To modify, edit the projects section in `index.html` or `Projects.jsx`

## 🎯 Figma-Style UI Design Prompt

**Design System:**
- Style: Modern Minimalist Portfolio
- Layout: Single-page, scroll-based navigation
- Grid: 12-column responsive grid
- Typography Scale: 3rem (hero) → 4rem (sections) → 1.125rem (body)
- Spacing Scale: 4px base unit (4, 8, 16, 24, 32, 48, 64, 96px)
- Border Radius: 8px (small), 12px (medium), 16px (large), 20px (xlarge)
- Shadows: 
  - Default: 0 4px 20px rgba(0,0,0,0.08)
  - Hover: 0 8px 30px rgba(0,0,0,0.12)
- Transitions: 0.3s cubic-bezier(0.4, 0, 0.2, 1)

**Component Specifications:**

1. **Navigation Bar**
   - Height: 64px
   - Background: rgba(255,255,255,0.95) with backdrop blur
   - Fixed position, top: 0
   - Shadow on scroll
   - Mobile: Hamburger menu

2. **Hero Section**
   - Full viewport height (100vh)
   - Two-column grid on desktop
   - Large typography: 5.5rem (desktop), responsive
   - Profile image: 400x400px, rounded corners, shadow
   - CTA buttons with hover states

3. **Section Headings**
   - Font size: 4rem (desktop)
   - Font weight: 800
   - Center aligned
   - Letter spacing: -1px
   - Margin bottom: 4rem

4. **Project Cards**
   - Grid: 3 columns (desktop), 1 column (mobile)
   - Card size: min 350px width
   - Image height: 250px
   - Hover: translateY(-8px) + shadow increase
   - Overlay on hover with action buttons

5. **Timeline**
   - Vertical line: 2px width
   - Marker: 16px circle with border
   - Content: Left-aligned with padding
   - Staggered animation on scroll

6. **Form Elements**
   - Border: 2px solid gray-200
   - Focus: Border color changes to black
   - Border radius: 8px
   - Padding: 1rem
   - Smooth transitions

## 📝 Portfolio Content

### About Section
Brief description of professional background, interests, and values. Highlights expertise in machine learning, web development, and data science.

### Skills
- Frontend: React, JavaScript, HTML/CSS, Tailwind CSS
- Backend & Data: Python, Node.js, Machine Learning, Data Science
- Tools: Git/GitHub, OpenCV, YOLO, Jupyter

### Projects (3 Types)
1. **AI/Computer Vision**: Real-Time Object Detection
2. **Web Development**: Weather Application
3. **Data Science**: AI Trend Forecast App

### Experience Timeline
- 2023 - Present: Full-Stack Developer & ML Engineer
- 2022 - 2023: Data Science & ML Projects
- 2021 - 2022: Web Developer
- 2020 - 2021: Learning & Foundation

### Testimonials
Three client testimonials highlighting different aspects of work (technical expertise, ML skills, web development).

## 🌐 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 📄 License

This project is open source and available for personal use.

## 👤 Author

**Yadavareddy Rohith**
- GitHub: [@RH1H](https://github.com/RH1H)
- Portfolio: [Live Site](your-portfolio-url.com)

---

Built with ❤️ using modern web technologies

