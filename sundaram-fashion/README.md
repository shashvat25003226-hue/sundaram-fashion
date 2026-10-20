# Sundaram Fashion — starter storefront

A responsive, no-build static storefront with catalog search, filters, product detail/size selection, wishlist, shopping bag, WhatsApp order enquiries, responsive navigation and Indian PIN-code postal lookup.

## Start
Open `index.html` in a browser, or serve the folder with `python -m http.server 8000` and visit `http://localhost:8000`. Upload this folder to any static host (Netlify, Vercel, GitHub Pages).

## IMPORTANT before publishing
1. **Replace all sample products** inside the `PRODUCTS` array in `index.html` with your own actual inventory, price, sizes, descriptions and **licensed product images**. Existing images are illustrative stock photography and may not match product names.
2. The WhatsApp number is configured as **+91 83193 98623**. Change all occurrences of `918319398623` if needed. Orders are **enquiries** — customer must tap Send in WhatsApp, then shop confirms stock, delivery and payment.
3. Replace generic About, Shipping/Returns, FAQs and Contact policy copy with verified business policies. Add a physical business address, GST details where applicable, official email, privacy policy, terms and refund policy before commercial launch.
4. Postal lookup uses the publicly accessible `api.postalpincode.in` endpoint (an independent third-party API with India Post directory information), with fallback to `api.pincodeapi.in`; **neither is an authenticated official India Post API**. To integrate an officially licensed India Post endpoint, replace `lookupPIN()` when credentials/endpoint are provided. Lookup does not imply courier serviceability.
5. Bag, wishlist and last order enquiry are saved in **this browser only**, using localStorage. There's **no database**, merchant admin portal, real multi-device accounts, secure order management, payment gateway, inventory syncing, email service, automated tracking, or AI assistant.
6. For a production full-commerce shop, add a secure backend (e.g. Supabase), authentication, admin product management, inventory and order storage, verified payment gateway (e.g. Razorpay), transactional notifications, and logistics/tracking integration.

## Features available in this starter
- Responsive home, collections and sample catalog
- Keyword search, category filtering, sorting, wishlist, product detail, sizes
- Shopping bag quantity controls and subtotal
- WhatsApp order enquiry builder with full shipping address
- PIN → post office, district and state lookup; manually editable when API unavailable
- FAQ, contact, basic shipping/returns explanation and enquiry support
- Keyboard Escape closing dialogs, labels, image lazy loading, basic input validation

This project is **not affiliated** with rivayat.shop and does not copy its protected branding or source code.
