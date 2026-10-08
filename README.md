# 1099 Hero website

The marketing site for the 1099 Hero iPhone app: https://1099hero.app

Plain static HTML and CSS. No build step, no JavaScript, no cookies, no analytics.
Hosted on GitHub Pages from the `main` branch (root folder).

## Layout

```
index.html            Home page (/)
support/index.html    Support + FAQ (/support/)  <- App Store "Support URL"
privacy/index.html    Privacy Policy (/privacy/) <- App Store "Privacy Policy URL"
404.html              Not-found page
assets/css/site.css   One shared stylesheet
assets/img/           Logo, icon, favicon, share image (og-image.png)
assets/img/screenshots/  App screenshots go here
```

Each page is its own folder so new sections (for example a future `/account/`)
can be added without changing existing URLs. All links are relative, so the site
works both at the GitHub Pages address and at the custom domain.

## Common edits

- **App Store launch:** in `index.html`, find the `AT LAUNCH` comment and swap the
  "Coming soon" text for Apple's official badge and the App Store link.
- **Screenshots:** put PNGs in `assets/img/screenshots/` and follow the
  `SCREENSHOTS` comment in `index.html`.
- **Privacy policy:** the text is a word-for-word copy of
  https://bobbyjones126.github.io/contractorhero-legal/privacy-policy.html.
  If you change one, change the other the same way.
- **Logo and icon files** are copied unchanged from the app's `/brand` folder.
  Don't edit them here.

## Wording rules

Never say "audit", "audit-proof", "guaranteed", "compliant", "correct", or
"IRS-approved", and never promise a tax result or savings amount.
