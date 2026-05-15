# MultiConstrucciones - Mantenimiento Residencial en Puebla

## Project Overview
Static HTML landing page for a residential maintenance and construction company in Puebla, Mexico. Single-file architecture with no build process required.

## Technologies
- **HTML5** with semantic markup
- **Tailwind CSS** (CDN-loaded)
- **Alpine.js** for lightweight interactivity (scroll reveal, count-up, modals)
- **Three.js** for 3D hero background animations (torus, octahedron, icosahedron)
- **DOMPurify** for form security

## Development Setup
- Open `index.html` directly in browser for testing
- For local server: `python -m http.server 8000` then visit `http://localhost:8000`
- No package manager or build tools needed

## Key Conventions
- **Language**: Spanish (es-MX) throughout
- **Responsive design**: Mobile-first with Tailwind breakpoints
- **Security**: CSP headers, input sanitization, honeypot spam protection
- **Performance**: Lazy loading with IntersectionObserver, staggered animations
- **Color scheme**: CSS variables `primary` (#2f855a verde bosque), `secondary` (#2b6cb0 azul océano), `accent` (#f6ad55 ámbar)
- **Animations**: Loader spinner, scroll reveal, count-up (Alpine.js), 3D wireframe (Three.js), hover effects

## Contact Info
- **Phone**: 222 255 3525
- **WhatsApp**: 522222553525
- **Address**: Bonampak 7A, La Rivera, San Andrés Cholula, Pue. CP 72813
- **Email**: info@multiconstrucciones.com
- **Services**: Jardinería, Pintura, Plomería, Electricidad, Impermeabilización, Albañilería, Lavado de Cisternas

## Common Tasks
- **Customize content**: Update service descriptions, contact info, images in index.html
- **Configure integrations**: Set up Formspree endpoint (line ~970), Calendly URL (line ~875), HubSpot forms
- **SEO optimization**: Update meta tags, schema.org structured data
- **Deployment**: Upload to static hosting (GitHub Pages, Netlify, Vercel)

## Pitfalls to Avoid
- Update Formspree ID (`YOUR_FORM_ID`) before going live
- Update Calendly URL (`tuusuario`) before going live
- Replace placeholder domain `multiconstrucciones.com` with real domain
- CDN dependencies may fail in restricted networks
- Schema.org address and geo coordinates are placeholders — verify before deployment

## Architecture Notes
- Single-page design with smooth scrolling navigation
- Component sections: Hero (3D), Trust Bar (count-up), Services (6 cards), About, Testimonials, Gallery, FAQ, Contact, Footer
- Alpine.js manages modal states, form validation, scroll animations, count-up
- Three.js renders 3 wireframe shapes rotating at different speeds
- Stagger delays on service cards (0–500ms) and gallery items (0–300ms)
- 800ms loader spinner on page entry</content>
<parameter name="filePath">c:\Users\gumod\Documents\Dev\Projects\MultiConstrucciones\AGENTS.md