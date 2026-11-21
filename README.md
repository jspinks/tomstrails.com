# tomstrails.com

Static site for Tomstrails apps, hosted on GitHub Pages. Plain HTML and one stylesheet: no build step, no JavaScript, no cookies.

## Files

| File | Served at | Notes |
|---|---|---|
| `index.html` | `/` | App overview |
| `gps-os.html` | `/gps-os` | GPS OS details and support |
| `gps-utm.html` | `/gps-utm` | GPS UTM details and support |
| `privacy.html` | `/privacy` | **Linked from App Store Connect — keep this path.** |
| `404.html` | any missing URL | Uses root-relative paths |
| `css/site.css` | | All styling, light and dark mode |
| `images/<app>/` | | `icon.png` and `screen-N.png` per app |
| `CNAME` | | Custom domain for GitHub Pages |
| `.nojekyll` | | Serve files as-is, no Jekyll |

GitHub Pages serves `name.html` at `/name`, so internal links use `.html` (works when opened locally) and the App Store's `/privacy` link still resolves. Don't add a top-level folder with the same name as a page.

## Preview

Open `index.html` in Safari. Use Develop → Enter Responsive Design Mode to check phone and tablet widths.

## Publish

Push to `main`; GitHub Pages deploys from the repository root.
