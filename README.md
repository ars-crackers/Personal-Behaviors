# தொழில்முனைவோர் சுய முன்னேற்ற கையேடு

தமிழில் ஒரு முழுமையான தொழில்முனைவோர் சுய முன்னேற்ற படிப்பு நூல் — 12 அத்தியாயங்கள், 14 விளக்கப்படங்கள், 90-நாள் செயல் திட்டம், சுய மதிப்பீட்டுக் கருவி.

A Tamil-language self-development study book for entrepreneurs. Static site, no build step, no dependencies.

## Files

| File | Purpose |
|---|---|
| `index.html` | Cover / landing page (this is what visitors see first) |
| `book.html` | The full 12-chapter study book |
| `guide.pdf` | Printable PDF version |
| `.nojekyll` | Tells GitHub Pages to serve files as-is |

## Publishing on GitHub Pages

1. Create a new repository on GitHub (public).
2. Upload all four files to the **root** of the repository — not inside a folder.
   Web upload: **Add file → Upload files → drag all files in → Commit changes**.
3. Go to **Settings → Pages**.
4. Under **Source**, choose **Deploy from a branch**.
5. Branch: `main`, folder: `/ (root)` → **Save**.
6. Wait about a minute, then open:
   `https://<your-username>.github.io/<your-repo-name>/`

`index.html` is served automatically as the homepage.

### Using the command line instead

```bash
git init
git add .
git commit -m "Add Tamil entrepreneur study book"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

Then enable Pages in **Settings → Pages** as described above.

## Notes

- Fonts load from Google Fonts. Offline, the browser falls back to a system Tamil font and everything stays readable.
- All diagrams are inline SVG, so there are no image files to break.
- To change the site title shown in search results and link previews, edit the `<title>` and `og:` meta tags at the top of `index.html`.
