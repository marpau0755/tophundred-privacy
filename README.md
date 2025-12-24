# Public Directory for Top Hundred

This directory contains the public-facing website files for the Top Hundred app, including:

## Files

- **index.html** - Marketing/landing page for the app
- **ads.txt** - Required by Google AdMob for ad verification
- **privacy-policy.html** - Privacy Policy (required for app store submissions)
- **terms-of-use.html** - Terms of Use (required for app store submissions)
- **README.md** - This file

## Deployment

This directory should be deployed to a public web server (e.g., GitHub Pages, Firebase Hosting, Netlify, or your own domain).

### Important Notes:

1. **ads.txt**: 
   - Must be placed at the root of your domain (e.g., `yourdomain.com/ads.txt`)
   - Replace `pub-0000000000000000` with your actual AdMob Publisher ID
   - You can find your Publisher ID in your AdMob account settings

2. **Privacy Policy & Terms of Use**:
   - Required by both Google Play Store and Apple App Store
   - Update contact email addresses in both files
   - Update jurisdiction information in Terms of Use (replace `[Your Jurisdiction]`)

3. **Domain Setup**:
   - When you have a domain, update the links in `index.html` to point to your app store listings
   - Ensure all links work correctly after deployment

## Customization

Before deploying, make sure to:

1. Update the AdMob Publisher ID in `ads.txt`
2. Update contact email addresses in `privacy-policy.html` and `terms-of-use.html`
3. Update jurisdiction information in `terms-of-use.html`
4. Customize the marketing page content in `index.html` if needed
5. Add your app store links when available

## GitHub Pages Setup

If using GitHub Pages:

1. Create a new public GitHub repository
2. Copy the contents of this `public` directory to the repository
3. Enable GitHub Pages in repository settings
4. Your site will be available at `https://yourusername.github.io/repository-name/`

## Firebase Hosting Setup

If using Firebase Hosting:

1. Install Firebase CLI: `npm install -g firebase-tools`
2. Login: `firebase login`
3. Initialize: `firebase init hosting`
4. Deploy: `firebase deploy --only hosting`

