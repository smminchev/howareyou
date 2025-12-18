# GitHub Pages Setup Instructions

## Current Status

✅ **Completed:**
- Privacy policy files created (English, Bulgarian, German)
- Git repository initialized
- Files committed to local repository
- Story marked as "Ready for Review"

⚠️ **Pending User Action:**
- Push repository to GitHub
- Enable GitHub Pages
- Verify deployment

---

## Step-by-Step Setup Guide

### Step 1: Create GitHub Repository

1. Go to https://github.com/new
2. Repository name: `whereareyou`
3. Description: "How Are You?! - Behavioral monitoring app for elderly safety"
4. Visibility: **Public** (required for GitHub Pages free tier)
5. Do NOT initialize with README, .gitignore, or license (we already have these)
6. Click "Create repository"

### Step 2: Push Local Repository to GitHub

In your terminal, run these commands:

```bash
cd C:\Users\Stoyan\whereareyou

# Add GitHub remote (replace [username] with your GitHub username)
git remote add origin https://github.com/[username]/whereareyou.git

# Push to GitHub
git push -u origin master
```

**Note:** GitHub may prompt for authentication. Use a Personal Access Token (PAT) instead of password.

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub: `https://github.com/[username]/whereareyou`
2. Click **Settings** (top navigation)
3. Click **Pages** (left sidebar)
4. Under "Source":
   - Branch: Select `master` (or `main` if that's your default branch)
   - Folder: Select `/docs`
5. Click **Save**
6. Wait 1-2 minutes for deployment

### Step 4: Verify Deployment

GitHub Pages will display a message:
> "Your site is published at `https://[username].github.io/whereareyou/`"

**Test the privacy policy URLs:**

1. English: `https://[username].github.io/whereareyou/privacy-policy.html`
2. Bulgarian: `https://[username].github.io/whereareyou/privacy-policy-bg.html`
3. German: `https://[username].github.io/whereareyou/privacy-policy-de.html`

Each page should load with:
- Proper formatting (centered, readable)
- Yellow disclaimer boxes
- All 9 sections visible
- Correct language (check lang attribute)

### Step 5: Update Google Play Console

Once URLs are live:

1. Copy the English privacy policy URL: `https://[username].github.io/whereareyou/privacy-policy.html`
2. Test it in a browser to confirm it's publicly accessible
3. Use this URL in Google Play Console Data Safety form
4. Reference `docs/google-play-data-safety-answers.md` for form responses

---

## Troubleshooting

### Issue: "404 Not Found" after enabling Pages

**Solution:** Wait 2-5 minutes. GitHub Pages can take time to propagate.

### Issue: Repository is private

**Solution:** GitHub Pages free tier requires public repositories. Go to Settings → General → Danger Zone → Change visibility → Make public.

### Issue: Wrong branch or folder selected

**Solution:** Go to Settings → Pages → Source and ensure:
- Branch: `master` (or your default branch)
- Folder: `/docs`

### Issue: Push requires authentication

**Solution:** Create a Personal Access Token:
1. GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Generate new token with `repo` scope
3. Use token as password when pushing

---

## Files Created

**Privacy Policy Files:**
- `docs/privacy-policy.html` - English (PRIMARY)
- `docs/privacy-policy-bg.html` - Bulgarian
- `docs/privacy-policy-de.html` - German
- `docs/README.md` - Documentation
- `docs/google-play-data-safety-answers.md` - Data Safety form guide

**Repository Files:**
- `.gitignore` - Android project gitignore
- `GITHUB-PAGES-SETUP.md` - This file

---

## Next Steps After Deployment

1. ✅ Verify all three language URLs are accessible
2. ✅ Test on mobile device (responsive design)
3. ✅ Run Google Lighthouse test (expect 90+ performance score)
4. ✅ Copy English URL for Google Play Console
5. ✅ Update story file with production URLs (replace `[username]` placeholders)

---

## Privacy Policy URL for Google Play

**Primary URL (English):**
```
https://[username].github.io/whereareyou/privacy-policy.html
```

**Data Safety Form Location:**
Google Play Console → App content → Privacy Policy → Add URL

**Required for:**
- Google Play Store submission
- Data Safety form (mandatory)
- Background location permission justification
- User trust and transparency

---

## Contact

**Developer:** Stoyan Shopov
**Email:** stoyan.shopov@gmail.com
**Story:** 1.1 Privacy Policy Creation and GitHub Pages Hosting
**Status:** Ready for Review
**Date:** 2025-12-18
