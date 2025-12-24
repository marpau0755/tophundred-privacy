# Deployment Guide for Top Hundred Public Site

## GitHub Repository Setup

Your public repository: https://github.com/marpau0755/tophundred-privacy.git

**IMPORTANT**: This repository is ONLY for the public website files (privacy policy, terms, marketing page). Do NOT push your mobile game code here.

---

## Quick Setup Steps

### 1. Navigate to Public Folder

```bash
cd public
```

### 2. Initialize Git Repository (if not already done)

```bash
git init
git remote add origin https://github.com/marpau0755/tophundred-privacy.git
```

### 3. Add Only Public Files

```bash
git add .
git commit -m "Initial commit: Privacy policy, terms of use, marketing page, and ads.txt"
git branch -M main
git push -u origin main
```

**Note**: Only files in the `public` folder will be pushed. The mobile game code stays in your private repository.

### 3. Enable GitHub Pages

1. Go to your repository: https://github.com/marpau0755/tophundred-privacy
2. Click **Settings** → **Pages**
3. Under **Source**, select **Deploy from a branch**
4. Select **main** branch and **/ (root)** folder
5. Click **Save**

Your site will be available at:
**https://marpau0755.github.io/tophundred-privacy/**

---

## Files Included

- `index.html` - Marketing/landing page
- `ads.txt` - Required by Google AdMob
- `privacy-policy.html` - Privacy Policy
- `terms-of-use.html` - Terms of Use
- `README.md` - This file

---

## Important: Update Before Deploying

### 1. Update `ads.txt`
- Replace `pub-0000000000000000` with your actual AdMob Publisher ID
- You can find this in your AdMob account settings

### 2. Update Contact Emails
- In `privacy-policy.html`: Replace `privacy@tophundred.app` with your actual email
- In `terms-of-use.html`: Replace `support@tophundred.app` with your actual email

### 3. Update Jurisdiction
- In `terms-of-use.html`: Replace `[Your Jurisdiction]` with your actual location (e.g., "California, United States")

---

## Custom Domain (Optional)

If you have a custom domain (e.g., `tophundred.app`):

1. Add a `CNAME` file to the repository root:
   ```
   tophundred.app
   ```

2. In GitHub Pages settings, add your custom domain

3. Update DNS records at your domain registrar:
   - Add a CNAME record pointing `tophundred.app` to `marpau0755.github.io`

4. **Important**: Update `ads.txt` to be accessible at `tophundred.app/ads.txt`

---

## Testing

After deployment, verify:
- ✅ `https://marpau0755.github.io/tophundred-privacy/` loads correctly
- ✅ `https://marpau0755.github.io/tophundred-privacy/ads.txt` is accessible
- ✅ `https://marpau0755.github.io/tophundred-privacy/privacy-policy.html` loads
- ✅ `https://marpau0755.github.io/tophundred-privacy/terms-of-use.html` loads
- ✅ All links work correctly

---

## App Store Submission

When submitting to app stores, use these URLs:

**Privacy Policy:**
```
https://marpau0755.github.io/tophundred-privacy/privacy-policy.html
```

**Terms of Use:**
```
https://marpau0755.github.io/tophundred-privacy/terms-of-use.html
```

**Support URL (optional):**
```
https://marpau0755.github.io/tophundred-privacy/
```

---

## Updating Files

To update files after initial deployment:

```bash
cd public
# Make your changes
git add .
git commit -m "Update privacy policy"  # or whatever changes you made
git push
```

Changes will be live within a few minutes on GitHub Pages.

