# Night Krawler Cleaning — Landing Page

A single-file, dependency-free landing page for a night-shift cleaning service.

## What's inside
- `index.html` — the entire site (HTML + CSS + JS in one file)
- `assets/hero-night.jpg` — hero background photo (user-supplied)
- `assets/logo.png` — recolored logo (amber + moon-blue on transparent background), used in the nav and footer
- `assets/melbourne-skyline.svg` — an original stylized skyline illustration used behind the contact section

## How to use
1. Open `index.html` in any browser to preview it locally — no build step needed.
2. To host it, upload the whole `night-krawler` folder (keep the `assets` folder alongside `index.html`) to any static host.
3. To edit content, open `index.html` in any text editor:
   - Hero headline/copy: inside the `<header class="hero">` section
   - Services grid: inside the `<section class="services">` section (each card has a `data-service` attribute — clicking it pre-fills the "What needs cleaning?" field with that text)
   - Contact details: inside the `<section id="contact">` section

## About the Melbourne background
I can't pull a real photo of Melbourne from the web into this file — most city photography online is copyrighted, and this is a live commercial site. Instead I built an original stylized skyline illustration (`assets/melbourne-skyline.svg`) in the site's amber/navy palette, referencing Melbourne's silhouette (a nod to the Eureka Tower's gold crown). If you have your own photo of Melbourne — one you've taken or licensed — send it over and I'll swap it in exactly like the hero photo.

## Enquiry form & email delivery
The form uses **FormSubmit** (https://formsubmit.co) to email submissions straight to `nightkrawlercleaning@gmail.com` — no backend or server required.

**Important — activation step:** the first time the form is submitted after deploying, FormSubmit sends a one-time confirmation email to `nightkrawlercleaning@gmail.com`. Someone needs to open that email and click the confirmation link — after that, every future submission is delivered automatically and silently.

The form includes:
- **Book now** and **Get a free quote** buttons in the hero — both jump to the form and preset the toggle (Book now → "Book now", Get a free quote → "Send enquiry"). Double check this matches what you intended — flag it if you want the mapping reversed.
- All fields (Name, Email, Phone, What needs cleaning) are required.
- On mobile, the services grid stays in a 2×2 layout rather than stacking to one column.

## Notes
- Fonts (Big Shoulders Display, IBM Plex Mono, Inter) load from Google Fonts via a `<link>` tag.
- Respects `prefers-reduced-motion` for the animated spotlight effect.
- Fully responsive down to mobile.
