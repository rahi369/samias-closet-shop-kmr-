# RahiVerse × SAMIA'S CLOSET — starter ZIP

A mobile-first, light-theme static web starter built from the supplied brief.

## Included and currently functional
- Responsive bilingual-ish storefront interface (Bengali default; EN toggle translates core navigation and headings)
- Brain Sprint quiz with 30 original questions, answer feedback, score, replay and share/copy fallback
- Fun personality quiz with deterministic category scoring
- Daily challenge, Bangladesh Standard Time date key, browser-local completion lock
- Product filters/search and demo inventory
- Cart quantities/totals with stock cap
- WhatsApp order-request link (does not claim order/payment confirmation)
- Style Studio filters using the current product list
- Reward and weekly reward sections that do not invent balances or countdowns
- Local-only demo product manager
- Responsive CSS and reduced-motion preference

## Important limitations — read before publishing
This is a functional **front-end starter**, not a migration of your private Base44 project. Your existing Base44 source code was not available, so this ZIP cannot preserve its database, auth, rewards, vouchers, orders or admin implementation automatically.

The product entries and Unsplash images are demo placeholders. Replace them with real product information and owner-provided images before selling. The WhatsApp number in `app.js` is set to `01314652599` from the conversation and must be confirmed before production.

The “Admin preview” is **not secure** and is not a production admin panel. It only changes local browser storage. Never rely on it to manage live orders, inventory, customer data or permissions. Production admin requires a real backend with server-side authentication, role checks and database rules.

Cart, demo products, and quiz history use `localStorage`; clearing browser data removes them. No payment gateway, database, real account system, real voucher wallet, persistent friend challenges, referral analytics, or verified order tracking is implemented in this static starter. Do not claim otherwise.

## Run locally
Open `index.html` in a browser. Some browser features (native sharing, clipboard) require HTTPS or a secure context. For normal hosting, upload the files to a static host such as Netlify or GitHub Pages.

## Connect Firebase (optional next phase)
The Firebase web configuration is public client configuration, not a security boundary. Before connecting a live database:
1. Enable only the Firebase products you actually need.
2. Configure Authentication providers.
3. Create role-based admin authorization that is enforced by Firestore Security Rules or trusted server code.
4. Ensure public visitors cannot read private orders or edit products.
5. Never place service-account keys or other privileged secrets in frontend files.
6. Test rules using Firebase Emulator/Rules Playground before publishing.

The Firebase config supplied in chat has intentionally not been embedded in this starter because no backend/security rules were supplied and the project is not yet connected.

## Replace demo inventory
For a quick local preview, use the footer's “Admin access” button. The demo passphrase is `local-demo`; this is deliberately only a local demonstration and offers no security. Products added this way stay in the current browser only. For production, build a secure admin workflow backed by a database.

## Publish
Upload the extracted folder to a static hosting provider. A published URL should only be shared after the provider confirms deployment. A static deployment does not add a database or secure admin automatically.

## Owner display
Owner: Md. Humaun Husen Rahi
Store: SAMIA'S CLOSET (men's and women's clothing)
Platform: RahiVerse
