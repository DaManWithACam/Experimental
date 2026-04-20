# Portfolio Website Specification

## Project Overview
- **Type**: Static photography/cinematography portfolio
- **Hosting**: GitHub Pages
- **Core functionality**: Showcase photography and video work with contact capability
- **Target users**: Potential clients, collaborators, fans

## UI/UX Specification

### Layout Structure
- **Single page** with smooth scroll sections
- Fixed navigation bar (becomes opaque on scroll)
- Sections: Hero, Gallery (Photos), Videos, About, Contact
- Responsive: mobile (<768px), tablet (768-1024px), desktop (>1024px)

### Visual Design

**Color Palette**
- Background: `#0a0a0a` (deep black)
- Surface: `#141414` (card backgrounds)
- Primary accent: `#e6c87a` (warm gold)
- Text primary: `#f5f5f5` (off-white)
- Text muted: `#888888` (gray)
- Border: `#2a2a2a`

**Typography**
- Headings: "Playfair Display", serif (elegant, editorial)
- Body: "DM Sans", sans-serif (modern, clean)
- Hero title: 72px desktop / 40px mobile
- Section titles: 48px desktop / 32px mobile
- Body: 16px, line-height 1.7

**Spacing**
- Section padding: 120px vertical (desktop), 80px (mobile)
- Container max-width: 1400px
- Gallery grid gap: 16px

**Visual Effects**
- Subtle grain texture overlay on hero
- Image hover: scale 1.03 with 0.4s ease
- Text reveal animations on scroll
- Smooth scroll behavior
- Navigation backdrop blur

### Components

**Navigation**
- Logo/name on left
- Links: Photos, Videos, About, Contact
- Mobile: hamburger menu with slide-in panel
- States: default (transparent), scrolled (solid background + blur)

**Hero Section**
- Full viewport height
- Large background image with dark overlay
- Title with staggered letter animation
- Subtitle with fade-in
- Scroll indicator (animated chevron)

**Photo Gallery**
- Masonry-style grid (CSS columns)
- Lightbox on click with navigation arrows
- Category filter tabs: All, Nature, Portrait, Urban, etc.
- Lazy loading images

**Video Gallery**
- Grid of video thumbnails with play overlay
- Embedded video player (click to expand)
- Support for YouTube/Vimeo embeds

**Social Links**
- Horizontal icons row
- Platforms: Instagram, YouTube, TikTok, Twitter/X
- Hover: gold color with subtle lift

**Contact Section**
- Simple form: Name, Email, Message
- Form submission via Formspree or similar (netlify forms compatible)
- Social links repeated here

**Footer**
- Minimal: copyright + back to top button

## Functionality Specification

### Core Features
1. Responsive navigation with mobile menu
2. Photo gallery with lightbox viewer
3. Video gallery (embedded players)
4. Contact form (ready for Formspree integration)
5. Smooth scroll navigation
6. Image lazy loading
7. Scroll-triggered animations

### Interactions
- Gallery filter: click tab, instant filter
- Lightbox: click image to open, arrows/esc to close
- Form: validation, submit button state
- Navigation: click scrolls to section

### Data Handling
- Images: placeholder paths (user adds later)
- Videos: YouTube/Vimeo embed IDs
- Form: Formspree endpoint placeholder

## Acceptance Criteria
- [ ] Site loads without errors
- [ ] All sections accessible from nav
- [ ] Photo gallery displays in masonry grid
- [ ] Lightbox opens and navigates correctly
- [ ] Videos play when clicked
- [ ] Contact form shows validation
- [ ] Mobile menu works
- [ ] Animations trigger on scroll
- [ ] Ready for GitHub Pages deployment