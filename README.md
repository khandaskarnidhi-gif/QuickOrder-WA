# QuickOrder WA 🛒💬
> Direct, zero-login WhatsApp storefront & ordering engine for local micro-merchants

[![Live Demo](https://img.shields.io/badge/Demo-Live%20Store-emerald)](https://khandaskarnidhi-gif.github.io/QuickOrder-WA/)

[Track] - Entrepreneurship & Local Business

Event - Kick To Tech

---

## 📌 Problem Statement
Millions of hyper-local micro-merchants (home bakers, cloud kitchens, tiffin providers, neighborhood kiranas) conduct daily business manually over WhatsApp chats[cite: 1]. 

Because standard messaging apps lack structured e-commerce tooling:
- Sellers deal with endless back-and-forth messages about item prices, availability, and addresses.
- Orders lead to manual calculation errors and overlooked custom requests (e.g., allergies, dietary preferences).
- Commercial aggregators (Zomato, Blinkit, Swiggy) impose 20–30% commissions, delayed weekly payouts, and rigid GST/KYC compliance that exclude informal micro-businesses.

---

## 💡 Solution: QuickOrder WA
**QuickOrder WA** is a lightweight, zero-login digital ordering application that bridges the gap between structured e-commerce catalogs and personal WhatsApp transactions[cite: 1]:

1. **60-Second Store Setup:** Merchants add their business name, WhatsApp number, and upload product photos directly from their device gallery (saved as Base64 in `localStorage`).
2. **Multi-Role URL Protection:** Generates a dedicated customer link (`?mode=customer`) that strips away admin controls so buyers cannot tamper with pricing or inventory[cite: 8].
3. **Smart Inventory Control:** Compulsory stock tracking with real-time stock deductions on order. Includes an urgent warning badge ("Only 2 left!") and a "🔔 Notify Me on WhatsApp" button when an item sells out.
4. **Flexible Fulfillment:** Customers choose between **Free Store Pickup (Takeaway)** or **Dynamic Home Delivery** with distance-based fees (0–3 km, 3–7 km, 7+ km).
5. **Instant Receipt Generation:** Converts the cart into an itemized, emoji-styled text receipt and triggers the merchant's WhatsApp chat (`wa.me`) with all details pre-filled.

---

## 🚀 Live Demo & Repository
- **Live Demo Link:** https://khandaskarnidhi-gif.github.io/QuickOrder-WA/
- **GitHub Repository:** https://github.com/khandaskarnidhi-gif/QuickOrder-WA

---

## 🛠️ Tech Stack & Architecture
- **Frontend:** Vanilla HTML5, Tailwind CSS (via CDN), Vanilla JavaScript (ES6+).
- **Storage & State:** Client-Side `localStorage` with URL query parameter parsing (`?mode=customer`)[cite: 8].
- **Integrations:** WhatsApp Universal Deep Link API (`https://wa.me/`).
- **Hosting:** GitHub Pages (Static Web Hosting)[cite: 6].
- **Zero Backend / Serverless:** 100% private and cost-free architecture with no external API keys or server subscriptions.

---

🤖 AI Tools Used & Prompting ApproachTools: 

Google Antigravity, v0 by Vercel, VS Code.  

Prompting Methodology: Structured prompt engineering leveraging the Role + Problem + User + Task + Constraints + Test Checklist pattern. 

Used iterative prompting for Base64 image compression, URL state isolation, and dynamic receipt formatting.

⚠️ Limitations & Future Scope

Current Limitations:

Inventory is stored client-side in the browser session rather than a centralized cloud database.

Payment verification relies on peer-to-peer UPI/Cash on Delivery confirmation rather than automated webhook callbacks.

Future Roadmap:

Lightweight Supabase integration for multi-device live cloud synchronization.

Dynamic UPI QR Code overlay (PhonePe/GPay) directly on checkout.

Multi-language support (Hindi, Marathi, Gujarati) for regional micro-vendors.

📜 Originality Declaration
This project was conceptualized, designed, and developed for PromptWars 2026 under the Entrepreneurship & Local Business track. All code logic, UI iterations, and architecture workflows have been thoroughly verified, tested, and understood by the team.

## 📋 How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/khandaskarnidhi-gif/QuickOrder-WA.git](https://github.com/khandaskarnidhi-gif/QuickOrder-WA.git)
   cd QuickOrder-WA
