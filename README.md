# Sangam Electricals — Website

A single-file static website. No backend, no database, no monthly costs.

---

## 📁 Folder Structure

When deployed to GitHub (or any host), your repo should look like this:

```
sangam-electricals-website/
├── index.html          ← The whole website (this one file)
├── README.md           ← This guide
└── images/             ← All project photos go here
    ├── luxury/         ← Bulgari, premium boutiques
    │   ├── 1.jpg
    │   ├── 2.jpg
    │   └── 3.jpg
    ├── watches/        ← Tissot, Seiko, Ethos, watch boutiques
    │   ├── 1.jpg
    │   └── 2.jpg
    ├── beauty/         ← Nykaa, beauty retail
    │   └── 1.jpg
    ├── fnb/            ← Subway, restaurants, F&B
    │   └── 1.jpg
    ├── fashion/        ← Fossil, apparel showrooms
    │   └── 1.jpg
    └── mattress/       ← Sleep Company, mattress D2C
        └── 1.jpg
```

---

## 📸 How to Add or Update Photos

**The HTML never needs to be edited again.** Just upload photos to the right folder.

1. Pick the right folder for the photo type (luxury, watches, beauty, fnb, fashion, mattress)
2. Name the photos **1.jpg, 2.jpg, 3.jpg ...** in order (no gaps — if you skip 3, it stops loading at 2)
3. Commit & push to GitHub — the site auto-detects the new photos and builds a slideshow

**Supported formats:** `.jpg`, `.jpeg`, `.png`, `.webp` (any of these works)

**Recommended specs:**
- Size: 1200 × 800 pixels (3:2 ratio looks best)
- File size: Under 500 KB each (compress at [tinypng.com](https://tinypng.com) if needed)
- Up to 10 photos per category

**What happens automatically:**
- If 1 photo: shows as a single image with circuit overlay
- If 2+ photos: builds a slideshow that auto-cycles every 4 seconds
- Shows "X PHOTOS" badge in the corner
- Adds little progress dots at the bottom

**If a folder has NO photos:** The card shows the stylized circuit diagram placeholder — still looks intentional and clean.

---

## 🚀 Deployment (GitHub Pages — Free Forever)

1. Go to [github.com](https://github.com) and create a new repository called `sangam-electricals` (or any name)
2. Upload `index.html` and the `images/` folder
3. Go to **Settings → Pages**
4. Under "Source," select **main branch / root**
5. Wait 1–2 minutes. Your site is live at `https://{your-username}.github.io/sangam-electricals/`

**To use a custom domain like `sangamelectricals.com`:**
- Buy the domain (~₹800/year on GoDaddy, Namecheap, or BigRock)
- In GitHub Pages settings, add the domain under "Custom domain"
- In your domain registrar's DNS settings, point it to GitHub Pages (instructions show up when you add the domain)

---

## ✏️ What to Edit if Content Changes

If you ever need to change actual text (not photos), open `index.html` in any text editor and search for:

| What to change | Search for | Where in file |
|----------------|------------|----------------|
| Phone number | `9000364477` | Multiple places |
| Email | `sangamelectricals2022@gmail.com` | Contact section |
| Service areas | `TELANGANA`, `ANDHRA PRADESH` etc. | Coverage section |
| Stats (years, states, services) | `11+`, `06`, `09` | Hero section |
| Service list | `New Construction Wiring` | Services section |
| Project descriptions | `Display lighting, showcase` | Projects section |

---

## 🎨 Design Notes

- **Color signature:** Electric yellow `#FFE800` on void black — distinctive, memorable, scales from mobile to desktop
- **Fonts:** Bricolage Grotesque (display) + Instrument Serif (italic accents) + JetBrains Mono (technical labels)
- **Interactions:** Glitch hover on hero, mouse spotlight (desktop), animated voltage lines, hover-to-light client tiles
- **Mobile-first:** Fully responsive, tap-to-call, WhatsApp float button, safe area for iPhone
- **Performance:** Single 72 KB HTML file. Fonts load from Google CDN. No images blocking initial render.

---

## ❓ Common Questions

**Q: Can I add more project categories beyond the 6?**
A: Yes — duplicate any `<div class="project-card" data-folder="...">` block in the HTML and give it a new folder name. Then create that folder under `images/`.

**Q: How do I change the order of slideshow photos?**
A: Just rename the files. The number in the filename is the order. So if you want a specific photo first, name it `1.jpg`.

**Q: What if a photo doesn't load?**
A: The card falls back to the stylized circuit graphic. Nothing breaks.

**Q: Does the WhatsApp button work?**
A: Yes. It opens WhatsApp on phones (or web.whatsapp.com on desktop) with a pre-filled message ready to send to 9000364477.

**Q: How does the project brief form send emails?**
A: It opens your default email app (Gmail on phone, Outlook on PC, etc.) with all the form data formatted as a structured email to sangamelectricals2022@gmail.com. The user just hits Send.

---

## 🛠️ Recommended Next Steps

1. **Buy the domain** — `sangamelectricals.com` or `.in`
2. **Deploy to GitHub Pages** (or Cloudflare Pages — also free)
3. **Set up Google Business Profile** for "Sangam Electricals Hyderabad" — free local SEO
4. **Add Google Analytics** if you want to see visitor stats (5 minutes to set up)
5. **Upload your best 3–5 photos per category** to start

---

Built with ⚡ in Hyderabad · 2025
