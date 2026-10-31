# Shopify Dawn CRO Supply-Pack Bundle Section (OS 2.0)

[![Live Demo](https://img.shields.io/badge/Live_Demo-ShopSideK_Hub-151413?style=for-the-badge&logo=vercel&logoColor=efe9de)](https://shopsidek-hub.vercel.app)
[![Shopify Dawn](https://img.shields.io/badge/Shopify-Dawn_OS_2.0-7AB55C?style=for-the-badge&logo=shopify&logoColor=white)](https://themes.shopify.com/themes/dawn)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)

A high-converting, native 1-3-6 quantity break bundle section engineered specifically for **Shopify Dawn (OS 2.0)**. 

Eliminates the need for bloated monthly bundle apps that inject 300KB+ of render-blocking JavaScript. Pure Liquid, native responsive CSS, and Vanilla JS connecting directly to Shopify's AJAX Cart API.

---

## Interactive Preview & AOV Simulators

Test the live interactive bundle picker and simulate your store's unit economics:
- **Interactive Teardown**: [https://shopsidek-hub.vercel.app](https://shopsidek-hub.vercel.app)
- **AOV & Gross Margin Calculators**: [https://shopsidek-hub.vercel.app/calculators](https://shopsidek-hub.vercel.app/calculators)

---

## Conversion Mechanics

```
┌────────────────────────────────────────────────────────┐
│ [1 Month Supply]   · 1 Bottle                          │
│ $49.00 ($49/ea)    · Full MSRP Anchor                  │
├────────────────────────────────────────────────────────┤
│ [3 Months Supply]  · ★ MOST POPULAR ★                  │
│ $117.00 ($39/ea)   · Save 20% (Default Selected Nudge) │
├────────────────────────────────────────────────────────┤
│ [6 Months Supply]  · 🏆 BEST VALUE                     │
│ $174.00 ($29/ea)   · Save 41% + Free Priority Shipping │
└────────────────────────────────────────────────────────┘
```

1. **Price Anchoring**: Pricing the 1-unit tier at full MSRP anchors perceived value.
2. **Default Selection Nudge**: Pre-selecting the 3-unit tier leverages loss aversion (downgrading feels like forfeiting a 20% discount).
3. **Micro-Commitment AJAX Add**: Instant `/cart/add.js` dispatch without full page reload.

---

## 60-Second Installation

### Step 1: Add the Liquid Section
1. In your Shopify Admin, navigate to **Online Store** → **Themes**.
2. Click **...** (three dots) next to Dawn → **Edit code**.
3. Under the **Sections** folder on the left sidebar, click **Add a new section**.
4. Name the file: `bundle-packs-cro.liquid`.
5. Copy the code from [`sections/bundle-packs-cro.liquid`](sections/bundle-packs-cro.liquid) and paste it into the editor.
6. Click **Save**.

### Step 2: Add to Product Template
1. Go to **Themes** → click **Customize** on Dawn.
2. At the top center dropdown, select **Products** → **Default product**.
3. On the left sidebar under **Template**, click **Add section**.
4. Search for **CRO Supply Packs Bundle** and select it.
5. In the right-side configuration panel:
   - Input your Shopify Variant IDs for each tier (1 Bottle, 3 Bottles, 6 Bottles).
   - Adjust headlines, badge text, savings percentages, and guarantee copy.
6. Drag the section directly below your product buy box or replace the standard variant picker.
7. Click **Save**.

---

## Technical Specifications

| Parameter | Specification |
| :--- | :--- |
| **Theme Compatibility** | Shopify Dawn 10.x, 11.x, 12.x, 13.x, 14.x (OS 2.0) |
| **External App Dependencies** | 0 (Zero external dependencies) |
| **Script Latency** | 0 ms (Inline vanilla JavaScript) |
| **Cart Integration** | Native Shopify AJAX API (`/cart/add.js`) |
| **Styling** | Scoped CSS, zero conflicts with theme styles |
| **Customizer Support** | Full Shopify Section Settings Schema |

---

## Automated Inventory & Multi-SKU Deductions

If your store pulls multi-pack inventory from single-unit stock automatically (without creating separate bundle variants in Shopify Admin), this section includes an optional hook to sync with **Kaching Bundles**.

Use partner code `SAVE20` for 20% off lifetime access:
- [Kaching Bundles on Shopify App Store](https://apps.shopify.com/bundle-deals?mref=fcmkmjly)

---

## Contributing & License

Contributions, issues, and feature requests are welcome!
Released under the [MIT License](LICENSE).
