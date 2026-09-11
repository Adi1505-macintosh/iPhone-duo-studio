# iPhone Duo Case Studio

Configure Apple's foldable — finish, official case, colour, angle — and take away a share card of exactly what you picked.

**→ [Try it](https://adi1505-macintosh.github.io/iPhone-duo-studio/)**

<br>

## What it does

Pick a **Star White** or **Night Sky** iPhone Duo. Leave it bare, or dress it in the **iPhone Duo Case** (Sand, Navy Blue) or the **iPhone Duo Folio with Kickstand** (Taupe, Navy Blue). Flip through every angle Apple photographed of that build — open, closed, back, kickstand — and open or close the Duo with one tap.

When you like what you see, the studio draws a 3:4 card of your build, tinted to your case colour, and hands it to you as a PNG you can post.

<br>

## One rule: no faked photography

This is the part that took the longest, and it's the part worth knowing about.

Apple doesn't photograph every case colour on every finish. Sand was shot on Star White; Navy on Night Sky. Filling the gaps would have meant recolouring pixels — swapping a white camera island for a dark one and calling it a product shot.

The studio doesn't do that. **Every image here is an unmodified Apple Store photograph.** The consequence is that some builds have more angles than others, so the interface tells you plainly — "4 Apple photos of this exact build" — and the share card reflows to suit. A build with one real photo gets one large frame rather than three repeats and a fabrication.

<br>

## Sharing

On a phone, **Share card** hands the PNG itself to the X or Threads app through the system share sheet — image and caption together, one tap.

On desktop, X and Threads only accept text through a link, so those buttons open the post with the caption ready *and* copy the card to your clipboard. Paste it into the composer to attach it. The file downloads as a backstop either way.

<br>

## Under the hood

One HTML file. No build step, no framework, no bundler, no dependencies, no analytics, no cookies, nothing sent anywhere. Your configuration is remembered in your own browser and nowhere else.

```
index.html      the entire page — markup, styles and logic
img/            26 product photographs (WebP) plus thumbnails
```

The share card is drawn on a `<canvas>` at 1536 × 2048. Each photo carries a pre-measured bounding box so tiles frame the product rather than the studio backdrop, whatever shape the shot is.

### Running it locally

Any static server will do — the card needs a real origin, so opening the file directly won't let it copy to the clipboard.

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

### Hosting your own

Drop the folder on GitHub Pages, Netlify, Cloudflare Pages or any static host. The share caption picks up whatever address it ends up on, automatically.

<br>

## Who made this

I'm **Aditya Darekar** — IT graduate, tech enthusiast, and someone who has spent rather too much of the last year thinking about folding phones. I write about Apple gear and how it actually fits into a day.

**[adityadarekar.medium.com](https://adityadarekar.medium.com)** · 2.8K readers

Two stories led directly to this project:

- [**Apple Finally Made A Device for Nerds Like Me — 7 Reasons The iPhone Duo Won Me Over**](https://medium.com/macoclock/apple-finally-made-a-device-for-nerds-like-me-7-reasons-the-iphone-duo-won-me-over-3a91500ec238?sk=a66b448052c4b790431d21fa706fbca1) — *Mac O'Clock, 12 min*
  An e‑reader, a notepad with Pencil support, a multitasking iPad — these are not three different devices. Not any more.

- [**One Week With The Fold 8 Has Me Excited For The iPhone Fold**](https://adityadarekar.medium.com/one-week-with-the-fold-8-has-me-excited-for-the-iphone-fold-33268c21622f?sk=dd1f6eb9d0bde7fa7abcad0ff9b83bc8) — *12 min*
  Living with Samsung's wider 4:3 fold for a week, and watching it quietly replace my iPad mini.

Both links are friend links, so there's no paywall.

<br>

## Credits

An unofficial concept, not affiliated with or endorsed by Apple. Product photography and specifications come from the [Apple Store](https://www.apple.com/shop/buy-iphone/iphone-duo) and the [iPhone Duo announcement](https://www.apple.com/newsroom/2026/09/apple-unveils-iphone-duo/) and remain © Apple Inc. Apple, iPhone, MagSafe and Ceramic Shield are trademarks of Apple Inc.
