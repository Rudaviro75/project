# PR helper and QA notes

This branch adds a shared header partial and improves the homepage hero selection.

Files added/changed:
- header.html (new shared header included via client-side fetch)
- assets/gallery/hero-1.svg (placeholder hero image: replace with a real photo at assets/gallery/hero-1.jpg)
- index.html (uses header include; adds preload + improved hero selection script)
- About.html, services.html, contact.html, admissions.html, Gallery.html, News and Events.html, Sports and Clubs.html (updated to use header include)
- css/styles.css (already updated in earlier commit)

QA checklist performed:
- Replaced per-page nav with a single shared header and client-side loader for consistency.
- Added a placeholder SVG hero so the homepage displays a background immediately.
- Updated hero selection script to prefer webp/jpg/svg and fall back to Unsplash if needed.

Next recommended steps:
- Replace assets/gallery/hero-1.svg with a real photograph (assets/gallery/hero-1.jpg or .webp). I can upload/optimize one if you provide it.
- Run visual checks on staging: mobile/desktop, keyboard focus, and contrast.

Testing notes:
- Checkout branch: git fetch && git checkout feature/navbar-hero
- Open index.html in a browser or serve the folder (python -m http.server 8000) and view http://localhost:8000

