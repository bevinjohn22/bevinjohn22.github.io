# Publishing your portfolio with a name-based URL

## Option 1 — Fastest: use your existing `portfolio` repository

URL after GitHub Pages is enabled: **https://bevinjohn22.github.io/portfolio/**

1. Sign in to `https://github.com/bevinjohn22`.
2. Open `https://github.com/bevinjohn22/portfolio` (this repository was empty at the time of preparation).
3. Select **Add file → Upload files**.
4. Extract the portfolio ZIP on your computer. Upload `index.html`, `.nojekyll`, `README.md`, `DEPLOY.md`, **and the entire `assets` folder** while retaining the folder structure. GitHub's web uploader may require choosing the folder or using drag-and-drop; verify the repository contains `assets/styles.css`, `assets/app.js`, `assets/projects.js`, and `assets/favicon.svg`.
5. Commit to the `main` branch.
6. In the repository choose **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: main → Folder: /(root) → Save**.
7. After GitHub Pages finishes deploying, click **Visit site** in Pages settings. It should use the project URL above.

If your GitHub UI doesn't allow uploading a folder directly, upload the ZIP's extracted contents by dragging the selected files and folder onto the repository's upload page, or use GitHub Desktop. **Do not upload the ZIP itself as the website.**

## Option 2 — Cleaner, free URL: `bevinjohn22.github.io`

The website URL will be **https://bevinjohn22.github.io/** (assuming the account owns that exact Pages repository and publishes successfully).

1. Under your account `bevinjohn22`, create a **new public repository** named **`bevinjohn22.github.io`** exactly.
2. Upload the extracted files as described above, at the repository root. Commit.
3. Go to **Settings → Pages → Deploy from a branch → main → /(root) → Save**.
4. Once deployed, use **https://bevinjohn22.github.io/** for your resumes and LinkedIn.

This is the shortest **free** URL with your GitHub username in it. The other GitHub profile `bejohn45` remains linked from the popup, regardless of which account hosts the site.

## Option 3 — Your own domain, e.g. `bevinjohn.com`

Buy a domain from a registrar **after verifying it is available**; the example is not a claim that it is available or registered. GitHub Pages hosting is free; the custom domain requires a domain purchase/renewal.

1. Publish via Option 1 or 2 first.
2. In the repository choose **Settings → Pages → Custom domain** and enter your actual domain (for example, `www.bevinjohn.com`), then **Save**.
3. At your domain registrar create the DNS records GitHub prescribes. For a `www` subdomain, add a `CNAME`: host `www`, value `bevinjohn22.github.io` (not the repository path). For an apex domain like `bevinjohn.com`, follow GitHub's current A/AAAA or ALIAS/ANAME instructions rather than copying stale IP addresses.
4. Verify domain ownership in GitHub's account Pages settings when prompted or recommended. Wait for DNS propagation and successful HTTPS provisioning.
5. Enable **Enforce HTTPS** on the repository's Pages settings once available.

Official GitHub instructions:
- https://docs.github.com/en/pages/quickstart
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
- https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/verifying-your-custom-domain-for-github-pages

## Updating the site later

Upload your revised `index.html` or files under `assets/` to the same repository and commit. GitHub Pages automatically republishes. The hash-based project URLs (`#/work/veil`, `#/work/codex`) work under either `/portfolio/` or the repository-root domain without server-side route configuration.
