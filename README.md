# Privacy Policy Hosting Guide (GitHub Pages)

This guide walks you through publishing the **PicMosaic: Grid, Frames & Art** Privacy Policy to **GitHub Pages** so you can paste the URL directly into your **Google Play Console** app listing.

---

## Step 1: Create a GitHub Repository

1. Log into your GitHub account: [github.com](https://github.com/)
2. Click **New Repository** (`+` in top-right).
3. Name your repository (e.g., `picmosaic-privacy-policy` or `privacy-policy`).
4. Set the repository visibility to **Public** (required for free GitHub Pages).
5. Leave "Add a README file" unchecked (or checked, either is fine), then click **Create repository**.

---

## Step 2: Push or Upload `index.html`

### Option A: Via GitHub Web Interface (Easiest / 1 Minute)
1. On your newly created GitHub repository page, click **Add file** &rarr; **Upload files**.
2. Drag and drop the [index.html](file:///e:/Workspace_Publish/PicMosaic/privacy_policy/index.html) file located at:
   `e:\Workspace_Publish\PicMosaic\privacy_policy\index.html`
3. Click **Commit changes**.

### Option B: Via Git Command Line (Ubuntu WSL)
Open WSL and run:
```bash
cd "/mnt/e/Workspace_Publish/PicMosaic/privacy_policy"
git init
git add index.html
git commit -m "Initial commit of PicMosaic Privacy Policy"
git branch -M main
git remote add origin https://github.com/<YOUR_GITHUB_USERNAME>/picmosaic-privacy-policy.git
git push -u origin main
```

---

## Step 3: Enable GitHub Pages

1. In your GitHub repository, navigate to **Settings** (tab at the top).
2. On the left sidebar menu, click **Pages** (under the "Code and automation" section).
3. Under **Build and deployment &rarr; Branch**:
   - Change `None` to **`main`** (or `master`).
   - Leave the folder as **`/(root)`**.
4. Click **Save**.
5. Wait ~30 to 60 seconds. Refresh the page until a green box appears:
   > *"Your site is live at `https://<YOUR_GITHUB_USERNAME>.github.io/picmosaic-privacy-policy/`"*

---

## Step 4: Add URL to Google Play Console

1. Open your **Google Play Console** &rarr; select **PicMosaic: Grid, Frames & Art**.
2. In the left navigation, scroll down to **Policy & programs &rarr; App content**.
3. Under **Privacy Policy**, click **Manage** or **Start**.
4. Paste your live GitHub Pages URL:
   `https://<YOUR_GITHUB_USERNAME>.github.io/picmosaic-privacy-policy/`
5. Click **Save**.
