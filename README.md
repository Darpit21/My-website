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

https://darpit21.github.io/My-website/

## Pages

| Page | Description |
| --- | --- |
| **Home** (`Ankita Dgitech.dc.html`) | The main one-page site, with sections for About, Services, Courses, Why Choose Us, Portfolio, Testimonials, and Contact. Includes a light/dark theme switch and a contact form that sends the enquiry through WhatsApp. |
| **Login** (`Login.dc.html`) | A sign-in and sign-up page for the Client & Student Portal, with two account types: Business Client and Course Student. |

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
| `index.html` | The home page entry point. GitHub Pages opens this first, and it redirects visitors to `Ankita Dgitech.dc.html`. |
| `Ankita Dgitech.dc.html` | The main website page (all the content above). |
| `Login.dc.html` | The login and sign-up page. |
| `support.js` | The runtime that renders both pages. It reads the `{{ ... }}` parts of the HTML and turns them into the finished page. Required — the site will not display without it. |
| `image-slot.js` | A helper component for drag-and-drop image placeholders, loaded by the home page. |
| `assets/` | The site's images: `logo.jpeg` (used in the header and footer of both pages), `akash-kashyap.jpeg`, and `raj-arpit.png` (team photos). |
| `.nojekyll` | Tells GitHub Pages to publish the files exactly as they are. Without it, GitHub's Jekyll processor can strip out the `{{ ... }}` code that `support.js` needs, leaving a blank page. Do not delete this file. |

The pages need an internet connection to display, because `support.js` loads React from a
public CDN (unpkg.com) when the page opens.

## How it was made

- **Designed with Claude Design**, which produced the `.dc.html` pages and the
  `support.js` / `image-slot.js` runtime files.
- **Hosted on GitHub Pages**, served from the `main` branch, root (`/`) folder.

## How to update

1. Edit the files in this folder — either by hand, or by asking Claude Code to make the
   change for you.
2. Save and commit your changes:
   ```bash
   git add -A
   git commit -m "Describe what you changed"
   ```
3. Push to GitHub:
   ```bash
   git push origin main
   ```
4. Wait 1–2 minutes. GitHub Pages rebuilds automatically, and your changes appear at
   https://darpit21.github.io/My-website/

If you do not see the update, do a hard refresh in your browser (Cmd + Shift + R on Mac,
Ctrl + Shift + R on Windows) to clear the cached old version.

### Adding or replacing images

Put the image file in the `assets/` folder, then point to it from the page with a path
like `assets/your-image.jpeg`. Keep the file name exactly the same as the one used in the
HTML — GitHub Pages treats uppercase and lowercase as different.

### A note on links

If you add a link to a file whose name contains a space, write the space as `%20`.
For example, `Ankita Dgitech.dc.html` must be linked as `Ankita%20Dgitech.dc.html`.
