# Cloth & Paper Wrapped: customer stats tool

One page (`index.html`) that turns Shopify exports into each top customer's Wrapped stats, in the browser. No Python, no installs.

**Upload:** the Shopify order exports, the wholesale and Faire customer lists, and optionally a products export (for top category) and a Yotpo Loyalty export (for loyalty tier).

**Download:** `wrapped_top100_for_team.csv`, one row per top customer with:
- rank, email and first name
- customer since and total orders
- items per order and Intention Boxes received
- top product, top category and go-to size
- first order of the year, loyalty tier and busiest month

Everything runs on the user's computer. The page makes no network requests, and customer data is never uploaded anywhere. The repository holds only the page, never data files.

## Hosting
GitHub Pages serves `index.html` from the repository root (Settings, then Pages, Deploy from a branch, main, / (root)). No GitHub? Download `index.html` and double-click it. It works offline.

Never commit export files or CSV results to the repository.

## Changing the rules
The rules (wholesale tags, box product names, planner sizes) are in the `RULES` block near the top of the script in `index.html`.
