# Cloth & Paper Wrapped: web tool

Three pages that build the Wrapped files in the browser. No Python, no installs.

- **index.html (Step 1):** upload the Shopify order exports, then download `wrapped_top400.csv`.
- **exports.html (Step 2):** upload `wrapped_top400.csv`, then download `klaviyo_import.csv` (and optional `canva_batch` files).
- **cards.html (Step 3):** make one shareable poster per customer (ZIP of PNGs) and get the HTML to paste into the Klaviyo email.

Everything runs on the user's computer. The pages make no network requests, and customer data is never uploaded anywhere. The repository holds only these pages, never data files.

## Put it on GitHub Pages
1. On GitHub, create a new repository, for example `cp-wrapped`, under the company account.
2. Click **Add file**, then **Upload files**, and upload `index.html`, `exports.html`, `cards.html` and this README. Then click **Commit changes**.
3. Go to **Settings**, then **Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main**, and folder to **/ (root)**. Click **Save**.
4. After a minute, the site is live at `https://<account>.github.io/cp-wrapped/`. Share that link.

Notes:
- GitHub Pages is free for public repositories. A private repository needs a paid GitHub plan. A public repo only shows the tool's code, not any customer data.
- No GitHub? Download the two files into one folder and double-click `index.html`. It works offline.
- Never commit export files or CSV results to the repository.

## Changing the rules
The rules (wholesale tags, box product names, planner sizes) are in the `RULES` block near the top of the script in `index.html`. Edit them there.
