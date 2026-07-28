# Bonfire at The Continental Fire Co.

Landing page for **Bonfire at The Continental Fire Co.**, a steakhouse, lounge, and live-music venue in a historic 1885 firehouse in downtown Houghton, Michigan.

A single, self-contained static site: one `index.html` with all CSS and JavaScript inline and photos embedded, plus one social-share image. No build step and no dependencies.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The complete landing page (styles, scripts, and most images inlined). |
| `bonfire-og.jpg` | 1200x630 Open Graph / social-share thumbnail. |
| `.gitignore` | Ignores common OS/editor junk files. |

## Deploy with GitHub Pages

1. Push these files to the repository root (`main` branch).
2. In the repo, go to **Settings -> Pages**.
3. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose `main` and `/ (root)`, then **Save**.
4. After a minute the site will be live at:

   ```
   https://velosify.github.io/bonfire/
   ```

The social-share tags in `index.html` already point at that URL. If you serve the site from a **custom domain** (or a different host such as Cloudflare Pages), update the absolute URLs in the `og:image`, `twitter:image`, and `og:url` meta tags near the top of `index.html` to match your final domain, or previews may not render.

## Local preview

Open `index.html` directly in a browser, or serve the folder:

```
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Editing notes

- **Menu** items and prices live in the `#menu` section, grouped by category (`.menu-cat`). All content is real as of the latest menu provided.
- **Reservations** use `tel:` links to (906) 523-5833. Update the number in the `href="tel:..."` links and the visible text if it changes.
- **Photos**: the Live Music and Story images and the OG thumbnail are real. The hero background, the four bar-category tiles, and the five Facebook tiles still use placeholder stock images. Replace those `url(...)` / `src=...` references with real photos when available.
- **Social**: the Facebook links point to <https://www.facebook.com/bonfire.cfc/>.
