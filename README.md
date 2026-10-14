# Ankita Dgitech – Website

Ankita Dgitech is an AI-based digital marketing agency in Patna, Bihar, helping local
businesses grow online with strategy, automation, paid media, design, and
conversion-focused digital experiences.

The agency combines creative storytelling, AI optimization, and local market insight to
help businesses stand out, capture stronger leads, and build marketing systems that keep
working after launch. While rooted in Patna, Bihar, its services are not limited by
location — it works with businesses across Bihar and all over India.

**Tagline:** Smart Marketing. Smarter Automation.

## Live website

Coming soon on our company domain.

## Pages

| Page | Description |
| --- | --- |
| **Home** (`index.html`) | The main one-page site, with sections for About, Services, Courses, Why Choose Us, Portfolio, Testimonials, and Contact. Includes a light/dark theme switch and a contact form that sends the enquiry through WhatsApp. |
| **Login** (`login.html`) | A sign-in and sign-up page for the Client & Student Portal, with two account types: Business Client and Course Student. |

Note: the Login page is currently front-end only. It checks that the password is at
least 6 characters and then shows a confirmation message. There is no server behind it
yet, so it does not actually create accounts or sign anyone in.

## Services

As listed on the website:

- Social Media Marketing
- Website Designing
- Meta Ads
- Google Ads
- SEO
- Snapchat Ads
- Branding & Designing
- WhatsApp Automation
- AI Automation
- Lead Generation
- Promotional Calls System
- Custom Call + Chat Bot

## Courses

- **Complete Digital Marketing Course** — 12 weeks, online + practical training
- **Kids Smart AI Course** — 4 weeks, beginner friendly
- **Complete AI Automation Course** — 12 weeks, online + practical training

## Team

| Name | Role |
| --- | --- |
| Raj Arpit | Founder & CEO |
| Ankita Bharti | Co-Founder |
| Akash Kashyap | Digital Marketing Manager |

## Contact

- **Email:** ankitadgitech@gmail.com
- **Phone:** +91 84092 10825
- **WhatsApp:** +91 84092 10825
- **Address:** Zero Mile, Jakariyapur, Patna-800007

Social profiles linked from the site: Instagram, Facebook, LinkedIn, and YouTube.

## Project files

| File / folder | What it is |
| --- | --- |
| `index.html` | The main website page (all the content above). This is the home page, and web servers open it automatically. |
| `login.html` | The login and sign-up page. |
| `support.js` | The runtime that renders both pages. It reads the `{{ ... }}` parts of the HTML and turns them into the finished page. Required — the site will not display without it. |
| `image-slot.js` | A helper component for drag-and-drop image placeholders, loaded by the home page. |
| `assets/` | The site's images — `logo.jpeg` (used in the header and footer of both pages), `akash-kashyap.jpeg` and `raj-arpit.png` (team photos) — plus the two React files below. |
| `assets/react.production.min.js`<br>`assets/react-dom.production.min.js` | React 18.3.1, stored locally so the site does not depend on an outside CDN. Both pages load these just before `support.js`, which then uses them instead of downloading React from the internet. Do not remove or rename these, and keep them loading before `support.js`. |
| `.nojekyll` | Only needed if the site is published with GitHub Pages — it stops GitHub stripping out the `{{ ... }}` code that `support.js` needs. It is harmless on Hostinger and other normal web hosts. |

### Outside connections

Everything the site needs in order to work is stored in this folder, so the pages build
and display without depending on any outside service.

The pages do still load a few things from the internet, but these only affect appearance.
If they are ever unavailable the site still works, just with fallback system fonts and
missing decorative pictures:

- **Google Fonts** — the Sora, Manrope and JetBrains Mono typefaces
- **Unsplash** — the portfolio photographs
- **jsDelivr, Simple Icons and unpkg (lucide-static)** — the small social, WhatsApp and
  chat button icons

## How it was made

- **Designed with Claude Design**, which produced the two pages and the
  `support.js` / `image-slot.js` runtime files.
- **Hosted on Hostinger**, on the company's own domain. This repository holds the master
  copy of the files.

## How to update

1. Edit the files in this folder — either by hand, or by asking Claude Code to make the
   change for you.
2. Save and commit your changes:
   ```bash
   git add -A
   git commit -m "Describe what you changed"
   ```
3. Push to GitHub, so the repository keeps the latest copy:
   ```bash
   git push origin main
   ```
4. Upload the changed files to Hostinger, into the `public_html` folder (using the
   Hostinger File Manager, or FTP). Keep the same folder layout, so `index.html`,
   `login.html`, `support.js`, `image-slot.js` and the whole `assets` folder (images and
   React files together) all sit in the same place.
5. Wait 1–2 minutes for the change to appear on the live domain.

If you do not see the update, do a hard refresh in your browser (Cmd + Shift + R on Mac,
Ctrl + Shift + R on Windows) to clear the cached old version.

### Adding or replacing images

Put the image file in the `assets/` folder, then point to it from the page with a path
like `assets/your-image.jpeg`. Keep the file name exactly the same as the one used in the
HTML — web servers treat uppercase and lowercase as different.

### A note on file names

Keep file names in lowercase with no spaces, as they are now. This avoids broken links on
the live server, since a space in a file name has to be written as `%20` in every link
that points to it.
