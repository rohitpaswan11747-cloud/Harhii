# Voda Feelpure — Storefront + Product Manager

## Quick open in Chrome
**Temporary browser preview:** https://raw.githack.com/rohitpaswan11747-cloud/Harhii/feature/voda-feelpure-store/index.html
**Catalog editor preview:** https://raw.githack.com/rohitpaswan11747-cloud/Harhii/feature/voda-feelpure-store/admin.html

The temporary URLs use a third-party preview proxy. For a permanent production URL, publish via GitHub Pages or your own hosting. Preview has not been verified to serve from the browser here.

## Add a product / change price (without coding)
1. Open **admin.html** in Chrome.
2. Choose a product (Edit) or New Product. Enter **name, SKU, category, price, image, and official buy link**.
3. Select a picture on your phone/computer using the image file picker; it is compressed and embedded into JSON, or paste an HTTPS image URL.
4. Press **Save Product**, then **Download products.json**.
5. In GitHub, open this branch's **products.json**. Tap pencil/Edit. Replace all text with downloaded products.json contents (or paste from **Copy JSON**) and **Commit changes**.
6. Refresh website preview; changes to catalog now display.

Important: the editor is browser-local and does *not* silently upload your images or change the live website. It has no password/login and exposes no sensitive server APIs. Only a GitHub commit publishes updates. Avoid putting personal or secret data in products.json; that file is public.

## How orders work
Buy buttons open Voda Chemicals' official product pages (https://vodachemicals.com/), where product options, carts and payment are handled. The new storefront never processes cards or payments. Prices are published starting/reference values (checked 21 Nov 2026) and can change or vary by variant. Contact form opens the device's email app.

## Public data sample
- Floor Cleaner (Lemon) from ₹79 (variants)
- Floor Cleaner (Rose) from ₹89
- Dish Wash Gel from ₹79
- Toilet Cleaner from ₹55
- Glass Cleaner from ₹70
- Bathroom Cleaner from ₹76
- Room Freshner from ₹195
- Tap Cleaner ₹199
- Complete Home Care Combo ₹480

**Confirm variants, images, prices, stock and ownership rights before public launch.** External image URLs may fail or require permission.

## Publish as a permanent site
1. In the repo GitHub settings, go to **Settings → Pages**.
2. Under Build and deployment, select **Deploy from a branch**. Choose `feature/voda-feelpure-store`, folder `/(root)`, then Save. (You need admin permission; repository is public.) 
3. GitHub Pages will show the URL once deployment finishes, typically `https://rohitpaswan11747-cloud.github.io/Harhii/` if Pages is enabled for this repo. **This URL is not currently verified live.**
4. When you later use `main` as the deployment branch, merge the review PR and update Pages source.

Note: GitHub Pages may restrict branch choice depending on repo settings; if so use the standard main branch after review. Check mobile experience and real images before launch.

## Current limits
No password-protected admin backend; no automatic product sync from WooCommerce, inventory, order database or independent Razorpay gateway. Those require a server/service connection and business account authorization.

## Verified source
https://vodachemicals.com/shop/
https://vodachemicals.com/product-category/housekeeping/homecare/
https://vodachemicals.com/product/complete-home-care-combo/
