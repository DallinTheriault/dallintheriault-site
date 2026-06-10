# Screenshots and images

The site ships with labeled SVG placeholders so the layout looks intentional before
you add real screenshots. Replace each placeholder with your own capture.

## How to swap one in

1. Capture the screenshot (specs below).
2. Save it into `images/` with the matching name, e.g. `images/field-cascade.png`.
3. In `index.html`, change that figure's `src` from `...svg` to `...png`.
   (Search the file for the filename, it's right above each screenshot.)
4. Commit and push. Netlify redeploys automatically.

PNG or JPG both work. Keep each file under ~500 KB if you can, so the page stays fast.

## What to capture

| File | Project | Tenant (demo data only) | Width | Notes |
| --- | --- | --- | --- | --- |
| `field-cascade.png` | Field | **Cascade** demo tenant | Desktop | Never Sharpline's real client data. Capture from `sharpline.getfield.co`. ~16:10. |
| `nillad-chat.png` | Nillad | n/a (your own machine) | Phone | The chat view. Nothing private in frame. |
| `field-pm-summit.png` | Field PM | **Summit Ridge Residential** | Phone | Demo tenant only, never the real wired property. Capture from `app.getfield.co` in Chrome device mode. |

## Optional: social preview image

For a nice LinkedIn/Twitter card, add `images/og-cover.png` (1200x630) and set the
absolute URLs in the `og:url` and `og:image` meta tags in `index.html` once your final
domain is live.

## Rules

- Demo tenants only. No real client names, no real resident data, no live phone numbers
  or infrastructure identifiers anywhere in frame.
