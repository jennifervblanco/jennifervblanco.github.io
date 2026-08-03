# Jennifer Blanco — Portfolio Website

A fast, static, multi-page portfolio built with plain HTML, CSS, and JavaScript. No build step, no framework. It is ready to deploy on GitHub Pages as-is.

## Deploy on GitHub Pages
1. Create a new GitHub repository (for a personal site you can name it `yourusername.github.io`, or use any name).
2. Upload every file in this folder, keeping the structure intact.
3. In the repo, go to **Settings → Pages**, set **Source** to the `main` branch and the root folder, and save.
4. Your site publishes at the URL GitHub shows (usually within a minute).
5. To use a custom domain, add a `CNAME` file containing your domain (for example `www.jenniferblanco.com`) and point your DNS at GitHub Pages.

## File structure
```
index.html            Home
work.html             Client work overview
case-rockwater.html   Case study
case-jcpower.html     Case study
case-blanco.html      Case study
strategy.html         Independent strategy concepts
photography.html      Photography, framed as a marketing skill
about.html            About
contact.html          Contact
404.html              Not-found page
assets/css/styles.css One stylesheet (the whole design system)
assets/js/main.js     One script (reveal, nav, small interactions)
assets/img/           Your images go here
assets/docs/          Resume PDF and the SeaWorld concept PDF
```

## How to edit
- All text lives directly in the HTML files. Search for the words you want to change.
- The header and footer are repeated in each page on purpose, so the site works without JavaScript and loads fast. If you change a nav link, update it in each page (a quick find and replace).
- Colors, fonts, and spacing are all controlled at the top of `assets/css/styles.css` under `:root`.

## CONTENT CHECKLIST (replace before sharing widely)
Everywhere you see a striped block labeled **Add photo** or **Add image**, drop the real file into `assets/img/` using the exact filename shown in that block. Priority order:

1. **Résumé PDF** → save as `assets/docs/jennifer-blanco-resume.pdf` (all Résumé links already point here).
2. **Hero portrait** → `assets/img/hero-portrait.jpg` (4:5, warm, editorial).
3. **Three work images** → `work-rockwater.jpg`, `work-jcpower.jpg`, `work-blanco.jpg` (4:3).
4. **Case study numbers** → in each case page, replace the bracketed `[ ]` metrics with real figures, ideally beside a dashboard screenshot.
5. **Photography** → the six category grids on `photography.html`, plus the five images on the home grid.
6. **Contact details** → search for `data-slot="email"`, `data-slot="linkedin"`, and `data-slot="booking"` and set your real email, LinkedIn URL, and booking link (Calendly or Cal.com). Do the same in each footer.
7. **Contact form** → create a free form at formspree.io and replace `YOUR_FORM_ID` in `contact.html`.
8. **Social share image** → `assets/img/og-image.jpg` (1200×630) for link previews.
9. **Testimonials** → optional but high value. If you gather two real quotes, tell me and I will add a testimonials section.

Nothing on the site uses fake data. Every place that needs a real asset is labeled.

## Notes
- Accessibility: semantic landmarks, a skip link, visible focus states, keyboard support, and reduced-motion handling are built in. Keep alt text descriptive when you add images.
- Performance: fonts load from Google Fonts. For maximum speed and privacy you can self-host the two font families later; the site works either way.
- The SeaWorld concept PDF is included at `assets/docs/seaworld-guest-experience-strategy.pdf` and linked from the Strategy page.
