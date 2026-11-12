NEXTY MINE — FINAL WEB BUILD

Repository: https://github.com/nextystudio1/NEXTY-MINE
GitHub Pages URL (after publishing): https://nextystudio1.github.io/NEXTY-MINE/

FILES
- index.html: complete player/admin web app, QRIS checkout UI, package orders and game rewards.

DATABASE / BACKEND ALREADY UPDATED
- Added nexty_payment_orders with owner-only player read access.
- Added nexty_create_payment_order(package_id): server determines the real package price.
- Added nexty_admin_review_payment(order_id, status): admin-only review; approval activates the package.
- Updated nexty-admin-overview Edge Function to include payment orders (version 3).

PACKAGE CATALOG CURRENTLY IN SUPABASE
- Free: Rp0
- Bronze: Rp20.000 / 7 hari
- Silver: Rp50.000 / 7 hari
- Gold: Rp100.000 / 7 hari
- Platinum: Rp250.000 / 7 hari
- Mythic: Rp500.000 / 7 hari

PUBLISH / UPDATE WEBSITE
1. Open https://github.com/nextystudio1/NEXTY-MINE
2. Open index.html, click the pencil/Edit button.
3. Replace all contents with index.html from this ZIP, then Commit changes to main.
   Alternatively delete the old index.html and upload the new one to the repository root.
4. Open Settings > Pages. Choose Deploy from a branch, branch main, folder /(root), then Save.
5. Wait for the Pages deployment to finish.

PAYMENT FLOW
- Player selects BUY; the backend creates a pending order using the package price stored in Supabase.
- The page shows the supplied Nexty Studio QRIS image and exact amount.
- Admin checks the actual merchant transaction record before selecting Approve & Activate or Reject.
- A screenshot or player claim alone is not proof of payment. Do not approve until the merchant dashboard confirms it.
- QRIS shown here is a static merchant QR. It does not automatically confirm payment; this build uses manual admin verification.
- Purchases must be handled with parent/guardian approval and by the authorized merchant owner. Do not collect or expose card/bank credentials.

GAME VALUE / REWARDS
- Gold is an in-game virtual point only. It does not represent rupiah, investment, income, or a promise to recover package cost.
- Reward redemption is limited to non-cash game items/features. There is no cash withdrawal or cash-out feature.

SECURITY
- Frontend contains only the Supabase anon key. Never put service_role/secret keys in index.html.
- Admin role is assigned only through Supabase app_metadata by the project owner. Public registration cannot grant admin access.
- Keep RLS enabled. Never mark a payment approved based only on a screenshot.
