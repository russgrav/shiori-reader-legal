# Setup Instructions

## Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com/new)
2. Create a new **public** repository named `shiori-reader-legal`
3. **Do not** initialize with README, .gitignore, or license (we already have them)
4. Click "Create repository"

## Step 2: Push to GitHub

```bash
cd "/Users/russellgraviet/Desktop/Personal Projects/shiori-reader-legal"
git remote add origin https://github.com/russgrav/shiori-reader-legal.git
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository settings: `https://github.com/russgrav/shiori-reader-legal/settings/pages`
2. Under "Source", select:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
3. Click "Save"
4. GitHub will deploy your site to: `https://russgrav.github.io/shiori-reader-legal/`

Wait a few minutes for deployment to complete.

## Step 4: Use in App Store Connect

Once GitHub Pages is live, use these URLs in App Store Connect:

### Privacy Policy URL
```
https://russgrav.github.io/shiori-reader-legal/privacy-policy.md
```

### Support URL
Choose one:
- GitHub Pages: `https://russgrav.github.io/shiori-reader-legal/`
- Direct email: `mailto:russgrav@gmail.com`

### Marketing URL (optional)
```
https://russgrav.github.io/shiori-reader-legal/
```

## What Apple Needs

For App Store Connect, you'll need to provide:

1. **Privacy Policy URL** (Required)
   - Must be publicly accessible
   - Should explain data practices
   - Ours states we don't collect any data

2. **Support URL** (Required)
   - Can be a website or mailto: link
   - We provide email support: russgrav@gmail.com

3. **Marketing URL** (Optional)
   - Can link to the legal docs page

4. **License** (Not required by Apple)
   - Included for transparency
   - MIT License shows open source components

## Updating the Documentation

To update any document:

1. Edit the file locally
2. Commit and push:
   ```bash
   git add .
   git commit -m "Update privacy policy"
   git push
   ```
3. GitHub Pages will automatically rebuild (takes 1-2 minutes)

## Testing

After GitHub Pages deploys, visit:
- Main page: https://russgrav.github.io/shiori-reader-legal/
- Privacy policy: https://russgrav.github.io/shiori-reader-legal/privacy-policy.md
- License: https://russgrav.github.io/shiori-reader-legal/LICENSE

Make sure all links work before submitting to Apple.
