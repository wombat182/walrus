# Walrus — site

Three pages plus a 404. HTML, CSS, and a small JavaScript animation on the home page.

## Files

- `index.html` — home (animated silhouette + wordmark + nav)
- `about.html` — company description + contact
- `walruses.html` — wild walrus photo placeholders
- `404.html` — graceful page for mistyped URLs
- `style.css` — all styling
- `walrus-logo.png` — silhouette only, transparent background, 3x resolution for retina

## Logo structure

The PNG is just the walrus silhouette — no wordmark, no background. The "walrus" text on the home page is real HTML in EB Garamond. So:

- Only the animal moves; the wordmark stays still
- No color mismatch possible (transparent background)
- Crisp on retina displays (logo is 3x display size)

## Animation

Just two things now:

1. **Breathe** — gentle continuous scale pulse
2. **Hop** — once every 35 seconds, the walrus does a quick cute hop. Slight crouch + lean back, jump up with a tilt forward, land and settle. ~1.3 seconds total. No horizontal movement.

Hover pauses everything and perks up the walrus. `prefers-reduced-motion` disables all motion.

## Editing

- **Email**: search `teigstad@icloud.com` in `about.html`
- **About paragraph**: edit `<p>` tags in `.content` div in `about.html`
- **Org.nr**: search `925&nbsp;629&nbsp;634` across HTML files
- **Partners link**: search `docs.google.com` in `index.html`
- **Add a photo**: in `walruses.html`, replace `<div class="placeholder">photo 1</div>` with `<img src="myphoto.jpg" alt="">`
- **Walrus size**: in `style.css`, find `#walrus-mark` and adjust `max-width` (currently 280px) or `width: 22vw`

## Colors

- Cream: `#F5EFE0`
- Brown: `#3E2C1C`
- Soft brown: `#6b5742`

## Future improvements

If you want a higher-quality logo, the right move is to convert the silhouette to SVG (vector) instead of PNG — then it'll be infinitely crisp at any size. Tools like Vector Magic or Adobe Illustrator's Image Trace can do this from your existing PNG.
