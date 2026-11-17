# Bridal Hairstyles by Alice — Demo Landing Page

A concept landing page for **Bridal Hairstyles by Alice** (Wilford, Nottingham), built by Codzo as a pitch demo.

The page tells the bride's story as she scrolls, from "Ciao, bella." to "Check your date". One silk ribbon draws itself through every chapter and ties into a bow at the booking form.

## Run it

There's no build step and nothing to install. It's one HTML file plus images.

```bash
# any static server works, e.g.
npx serve .
# or
python3 -m http.server 8000
```

Then open http://localhost:8000. You can also open `index.html` directly in a browser.

## Deploy

Works as-is on Vercel, Netlify, GitHub Pages or Cloudflare Pages. Point the project root at this folder.

## Structure

```
index.html   page, styles and scripts (vanilla JS, no libraries)
img/         client photos, cropped from her current website
```

## Chapters

| # | Section | Effect |
|---|---|---|
| — | Hero: *Ciao, bella.* | Words un-blur, olive branch draws, arch photo reveals |
| — | Pull line | Word-by-word un-blur |
| Uno | Meet Alice | Arch portrait, botanical sprig grows over the arch |
| Due | Your journey (4 steps) | Pinned section; photos open with a circular reveal |
| Tre | Behind the scenes | Reels slide sideways as you scroll |
| Quattro | Kind words | Rotating testimonials, un-blur |
| Cinque | The work, up close | Framed portfolio; the ribbon passes behind the photos |
| — | For the bride | Guide cards |
| Sei | Check your date | Service picker updates the side photo; the ribbon ties a bow |

Also on every page: a cursor petal trail (desktop only), mobile layouts, and a full `prefers-reduced-motion` fallback.

## Before going live

- [ ] Replace the `£___` and `2027` placeholders (marked with a dashed underline)
- [ ] Swap `img/alice.jpg` for a high-resolution portrait
- [ ] Replace the reel stills with Alice's real videos
- [ ] Alice to approve the journey copy (all quotes are from her real testimonials)
- [ ] Connect the booking form to email (it currently shows a thank-you state only)
- [ ] Add real social links in the footer

## Next (production)

Port each chapter to a Next.js component (`Hero`, `MeetAlice`, `Journey`, `Reels`, `KindWords`, `Work`, `Guides`, `Booking`, `Footer`), add `next/image`, and send the form through an email API.

---

Photos and testimonials belong to Bridal Hairstyles by Alice. Keep this repository **private**.
