# CURA Package Finder

A booth screening questionnaire for CURA: Bespoke Grooming & Wellness Aggregator. It asks what a customer needs and their maximum budget, then recommends a package with the final price.

It is one static file (`index.html`). No server, database or build step. Nothing a customer enters leaves their device.

## Put it online with GitHub Pages

1. Sign in at github.com and click **New repository**. Name it `cura-package-finder` and make it **Public**.
2. On the new repo page, click **uploading an existing file**. Drag in `index.html` and `README.md`, then click **Commit changes**.
3. Open **Settings > Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main** and folder to **/ (root)**, then click **Save**.
4. Wait about a minute and refresh. GitHub shows your link: `https://YOUR-USERNAME.github.io/cura-package-finder/`
5. Open the link on a phone and a tablet and run a full questionnaire.

## Use it at the booth

- Open the link on the booth tablet and choose **Add to Home Screen** for one-tap access.
- Make a QR code of the link (any free QR generator) and print it on the booth backdrop so students can try it on their own phones.
- Wi-Fi is only needed to load the page and the Google Fonts. If it is unreliable, download `index.html`, open it from the tablet's files, and it works offline with fallback fonts.

## Update prices

All prices are in the `<script>` section of `index.html`.

1. Open the file on GitHub and click the pencil icon.
2. Search for `PACKAGES` to change package prices and partner base costs.
3. Search for `function buildCustom` to change the partner rates used for custom builds.
4. Search for `FEE_PCT` and `FEE_FLAT` to change the custom service fee.
5. Click **Commit changes**. The site updates in about a minute.

Package prices and base costs come from the concept paper. Partner rates come from the CURA Partner Services Master Price List.

## Staff settings

Open **Staff settings** at the bottom of the page to switch the custom fee between 15% and PHP 100 per voucher, and to show partner cost and margin on the result.
