# FLEX∞ - Ultra-Premium 3D AMV Editor Portfolio

A production-quality cinematic portfolio website for FlexInfinity, an AMV editor and motion designer. Built with cutting-edge web technologies to deliver an immersive, interactive visual experience.

## 🎬 Features

### Visual Design
- **Dark & Minimal Aesthetic** - 90% black surfaces with electric blue accents (#1677FF)
- **3D Particle System** - Real-time WebGL particle field in hero using Three.js
- **Cinematic Effects** - Film grain, scanlines, chromatic aberration, blur transitions
- **Smooth Scrolling** - Lenis-powered physics-based scrolling with velocity detection
- **Parallax Depth** - Multi-layer background effects with mouse-tracking parallax

### Interactive Elements
- **Custom Cursor** - Desktop-only animated cursor with contextual states (project, video, drag, link, button)
- **Magnetic Interactions** - Buttons and links respond to cursor proximity
- **Scroll-Triggered Animations** - Content reveals as user scrolls through sections
- **Responsive Gallery** - Magazine-style project layout with hover effects and blue light sweeps
- **Interactive Video Player** - Custom controls with fade-in/out on inactivity

### Sections
1. **Loading Screen** - Cinematic loader with animated progress, particles, and scanlines
2. **Navigation** - Glass-morphism navbar with smooth transitions and mobile menu
3. **Hero** - Fullscreen 3D particle field with animated typography and CTAs
4. **Showreel** - Custom video player with cinematic frame borders
5. **Projects** - Interactive gallery with editorial magazine-style layout
6. **Skills** - Interactive toolkit selector with workflow timeline
7. **About** - Service cards, statistics, and personal statement
8. **Contact** - Form with validation and status feedback
9. **Footer** - Minimal footer with navigation and social links

### Performance Optimizations
- Lazy loading for images and videos
- GPU-accelerated animations (transform, opacity only)
- Dynamic imports for heavy libraries
- IntersectionObserver for viewport-triggered animations
- Reduced motion support for accessibility
- Mobile-optimized experience

## 🛠 Tech Stack

- **Framework**: React 18.3 + TypeScript
- **Build Tool**: Vite
- **Animation**: Framer Motion, GSAP
- **3D Graphics**: Three.js, React Three Fiber
- **Scrolling**: Lenis (smooth scroll library)
- **Styling**: Tailwind CSS
- **State Management**: Zustand
- **Icons**: Lucide React

## 📦 Installation

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## 📁 Project Structure

```
flexinfinity-portfolio/
├── src/
│   ├── components/        # React components
│   │   ├── Loader.tsx
│   │   ├── CustomCursor.tsx
│   │   ├── Navigation.tsx
│   │   ├── Hero.tsx       # 3D scene
│   │   ├── Showreel.tsx
│   │   ├── Projects.tsx
│   │   ├── Skills.tsx
│   │   ├── About.tsx
│   │   ├── Contact.tsx
│   │   ├── Footer.tsx
│   │   ├── Scene3D.tsx    # Three.js component
│   │   └── index.ts
│   ├── hooks/
│   │   └── useAnimation.ts    # Custom hooks
│   ├── store/
│   │   └── index.ts           # Zustand stores
│   ├── App.tsx
│   ├── main.tsx
│   └── index.css
├── index.html
├── vite.config.ts
├── tailwind.config.js
├── postcss.config.js
├── tsconfig.json
└── package.json
```

## 🎨 Design System

### Colors
- **Black**: `#030303` (background)
- **Dark**: `#080B10` (secondary surface)
- **Blue**: `#1677FF` (primary accent)
- **Light Blue**: `#4DA3FF` (hover/highlight)
- **White**: `#F5F7FA` (text)

### Typography
- **Headings**: System font stack, ultra-bold, tight tracking
- **Body**: System font stack, light weight
- **Mono**: Fira Code (for technical details)

### Animation Durations
- Fast: 150ms (micro-interactions)
- Normal: 300ms (standard transitions)
- Slow: 500ms (attention-drawing)
- Very Slow: 800ms (complex sequences)

## 🎮 Interactions

### Cursor States
- **Default** - Small white dot with blue ring
- **Project** - Ring expands, text shows "VIEW"
- **Video** - Text shows "PLAY"
- **Drag** - Text shows "⇄"
- **Link** - Text shows "↗"
- **Button** - Ring expands, subtle pull effect

### Scroll Behaviors
- Hero zooms and transitions as user scrolls away
- Content fades and scales in as viewport reaches sections
- Custom cursor responds to mouse movement
- Navigation bar gains glass effect after scroll threshold

### Mobile Experience
- Custom cursor disabled on touch devices
- Simplified animations for performance
- Fullscreen mobile menu with staggered animations
- Touch-optimized form inputs
- Vertical project gallery layout

## 🔧 Customization

### Update Content
Edit component files to customize:
- Project titles and descriptions in `Projects.tsx`
- Service offerings in `About.tsx`
- Skills and tools in `Skills.tsx`
- Social links in `Footer.tsx`

### Adjust Colors
Update colors in `tailwind.config.js`:
```javascript
colors: {
  blue: '#1677FF',
  'light-blue': '#4DA3FF',
  // ... etc
}
```

### Modify Animations
Adjust animation durations and easing in individual components or globally in `index.css`.

### Video & Images
Replace placeholder URLs in components:
- Hero: Update 3D scene or add background video
- Showreel: Replace video source in `Showreel.tsx`
- Projects: Update project images in `Projects.tsx`

## ♿ Accessibility

- Semantic HTML structure
- Keyboard navigation support
- Focus states on interactive elements
- ARIA labels for screen readers
- Respects `prefers-reduced-motion` media query
- Sufficient color contrast ratios
- Form labels and validation messages

## 📊 Performance Targets

- **Lighthouse**: 90+ score across metrics
- **Page Load**: < 3 seconds on 4G
- **Frame Rate**: 60 FPS on desktop, 30+ FPS on mobile
- **Time to Interactive**: < 2 seconds

## 🚀 Deployment

### Vercel (Recommended)
```bash
npm i -g vercel
vercel
```

### Netlify
```bash
npm run build
# Drag-and-drop dist/ folder to Netlify
```

### GitHub Pages
Update `vite.config.ts` with your repository name and run `npm run build`.

## 📝 Notes

- This portfolio uses placeholder content and images
- Replace all placeholder images with actual project screenshots
- Update social media links in Navigation and Footer
- The video player uses a placeholder video URL
- Form submission is frontend-only; integrate backend as needed

## 📄 License

© 2026 FlexInfinity. All rights reserved.

---

**Built with precision. One frame at a time.**
