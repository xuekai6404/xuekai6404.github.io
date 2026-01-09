# EtaNotes Website

This is the GitHub Pages website for EtaNotes, containing the product introduction page and app-ads.txt file.

## File Description

- `index.html` - Product introduction homepage
- `app-ads.txt` - Ad verification file (for Google AdMob)
- `assets/style.css` - Website stylesheet

## Deployment Instructions

### GitHub Pages Setup

1. In the GitHub repository, go to **Settings** > **Pages**
2. In the **Source** section, select:
   - Branch: `main` (or `master`)
   - Folder: `/docs/website`
3. Click **Save** to save the settings
4. The website will be deployed within a few minutes to: `https://[username].github.io/EtaNotes/`

### app-ads.txt Configuration

1. Open the `app-ads.txt` file
2. Replace `pub-XXXXXXXXXXXXXXXX` with your actual Google AdMob Publisher ID
3. The Publisher ID can be found in the [Google AdMob Console](https://apps.admob.com/) under **Settings** > **Account Information**
4. After submitting changes, the file will be automatically deployed

### Verify app-ads.txt

After deployment, you can verify it by:

1. Visit: `https://[username].github.io/EtaNotes/app-ads.txt`
2. Confirm that the file is accessible and the content is correct
3. Verify domain ownership in Google AdMob (if required)

## Update Download Links

Update the actual App Store and Google Play download links in `index.html`:

- iOS download link: Find the `<a>` tag with `id="ios-download"`, update the `href` attribute
- Android download link: Find the `<a>` tag with `id="android-download"`, update the `href` attribute

## Notes

- After updating the app-ads.txt file, it may take several hours for ad networks to crawl it
- Ensure HTTPS access is used (GitHub Pages provides this automatically)
- If you need to use a custom domain, configure it in the GitHub Pages settings
