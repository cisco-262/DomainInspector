# DomainName Website

This folder contains the static marketing and support website for DomainName.

## Structure

- `index.html` - English homepage.
- `zh-cn/index.html` - Chinese homepage.
- `privacy/index.html` - English privacy policy.
- `terms/index.html` - English terms of use.
- `support/index.html` - English support page.
- `zh-cn/privacy/index.html` - Chinese privacy policy.
- `zh-cn/terms/index.html` - Chinese terms of use.
- `zh-cn/support/index.html` - Chinese support page.
- `styles.css` - Shared site styles.
- `assets/images/` - App logo, favicons, touch icons, manifest icons, and Open Graph image.
- `favicon.ico` - Browser favicon.
- `site.webmanifest` - Web app icon manifest.
- `og.png` - Open Graph preview image.
- `IMG_0544-portrait.png` - Homepage app screenshot.

## Language Pages

The English and Chinese pages are independent static pages. The language switcher uses normal links:

- English homepage links to `./zh-cn/`.
- Chinese homepage links to `../index.html`.
- Policy and support pages link to their matching language versions.

Do not reintroduce JavaScript text replacement for language switching. Keep each language page as its own HTML file so page titles, metadata, content, and links can be maintained independently.

## Support Email

The support email shown on the site is:

`support@opshome.run`

When changing the support address, update all `mailto:` links and visible email text across both English and Chinese pages.

## Assets

Primary app and browser assets are stored in `assets/images/`:

- `app-logo.png`
- `apple-touch-icon.png`
- `favicon-16.png`
- `favicon-32.png`
- `icon-192.png`
- `icon-512.png`
- `og.png`

The root `favicon.ico`, `site.webmanifest`, and homepage images should stay in sync with these assets when the app branding changes.

## Local Preview

This is a static website. You can preview it by opening `index.html` in a browser, or by serving the folder with any static file server.

Example:

```bash
python -m http.server 8080
```

Then open:

`http://localhost:8080/`
