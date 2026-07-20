# Lantern Watch — Website

Marketing site for **Lantern Watch**, a free, open-source family network-safety app
that runs on your own router. Content filtering, parental controls, and screen-time
limits — local-first, no subscription, no cloud surveillance.

🔗 Live: <https://lanternwatch.org> · App: <https://github.com/LanternWatchApp/lantern-watch>

## What's here

Plain static HTML/CSS — no build step, no framework, no dependencies.

```
.
├─ index.html        # Main page (hero, features, how it works, demo, routers, contact)
├─ compare.html      # Feature comparison vs other parental-control tools
├─ CNAME             # Custom domain for GitHub Pages
└─ assets/images/
   └─ lantern.svg    # Logo
```

## Local preview

Just open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 8000   # then visit http://localhost:8000
```

## Deploy (GitHub Pages)

Pushed to `main` → **Settings → Pages → Deploy from branch → main / root**.
The `CNAME` file points the site at `lanternwatch.org`.

## Contact form

The form on `index.html` posts to [Formspree](https://formspree.io). Replace
`YOUR_FORM_ID` in the form's `action` with your Formspree form ID. Spam protection
is configured in the Formspree dashboard.

## License

[MIT](LICENSE) © Lantern Watch
