# Chloe Kim — Portfolio Website

A static site (plain HTML, CSS and JS) with nothing to build. It's ready for GitHub Pages and a custom domain.

## Pages
| File | Section |
|---|---|
| `index.html` | Home: brand, value proposition, headshot |
| `about.html` | About Me / My Story |
| `experience.html` | Work & internships, software proficiency |
| `resume.html` | Embedded + downloadable resume |
| `education.html` | UMD Smith School, courses, writing sample, Strategic Design Fellows |
| `portfolio.html` | Case studies (problem → challenges → process → outcome, creative brief) |
| `blog.html`, `post-*.html` | Two blog posts |
| `contact.html` | Contact info + working contact form |

## Editing
- Text in `[square brackets]` is placeholder copy. Replace it with your own.
- Look for `<!-- EDIT: -->` comments for guidance.
- **Resume:** replace `assets/docs/Chloe-Kim-Resume.pdf` with your PDF (same name).
- **Writing sample:** replace `assets/docs/writing-sample.pdf`.
- **Software levels:** in `experience.html`, set the label (Expert/Advanced/Intermediate/Beginner) and the bar `width` (95% / 78% / 55% / 30%).
- **Colors/fonts:** all brand tokens are at the top of `assets/css/style.css`.

## Publish on GitHub Pages
1. Create a new repository on GitHub (e.g. `portfolio`) and upload all files, or push with git:
   ```bash
   git remote add origin https://github.com/<your-username>/portfolio.git
   git push -u origin main
   ```
2. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch → `main` / `(root)` → Save**.
3. Your site goes live at `https://<your-username>.github.io/portfolio/` within a minute or two.

Every time you commit and push a change, the site updates automatically.

## Connect your own domain
1. **Settings → Pages → Custom domain:** enter `www.yourdomain.com` and save. (This creates a `CNAME` file in the repo.)
2. At your domain registrar (GoDaddy, Squarespace, Namecheap, etc.), add DNS records:
   - `CNAME` record: host `www` → `<your-username>.github.io`
   - `A` records for the root domain (`@`) → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
3. Once DNS is verified, check **Enforce HTTPS**.

## Contact form
The form uses [FormSubmit](https://formsubmit.co) (free, no account). The **first** message sent from the live site triggers a confirmation email to kim.d.chloe@gmail.com. Click the link in it once, and every message after that goes straight to your inbox.

## Preview locally
Open `index.html` in a browser, or run `python3 -m http.server` in this folder and visit http://localhost:8000.
