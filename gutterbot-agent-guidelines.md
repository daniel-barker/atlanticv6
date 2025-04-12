# Atlantic Gutter Supply AI Agent Instructions

---

## 🤖 Agent Name
**GutterBot**  
*Mission: Modernize Atlantic Gutter Supply’s web presence and help sell hella gutters.*

---

## 📌 Project Context
Atlantic Gutter Supply is a long-established supplier of gutter materials and tools. The website:
- Is outdated and lacks mobile responsiveness
- Needs a new structure, look, and dynamic product catalog
- Should reflect **quality, service, and value**

---

## 🛠️ Technical Stack
- **Framework**: SvelteKit + Tailwind CSS v4
- **Backend**: Firebase (Firestore + Auth)
- **Storage**: Firebase Storage (or Cloudinary if needed)
- **Hosting**: Vercel

---

## 🧭 Project Principles
1. **No Bloat** – Simple, clean code. No unnecessary frameworks or files.
2. **Gutter-Centric UX** – Prioritize users looking for gutter products or services.
3. **Admin-Friendly** – CRUD should feel like a breeze.
4. **Mobile First** – Everything must look tight on phones.
5. **Branded but Functional** – Lean into the logo’s vibe and color palette without overdesigning.

---

## 📚 Content Guidelines
- Use copy that’s direct, helpful, and confident.
- Avoid buzzwords; stick to construction/equipment lingo.
- Highlight:
  - Material selection
  - Delivery capability
  - Tooling and machine service
  - Install guidance for contractors

---

## 🧩 Components to Build

### Global Layout
- Header with nav
- Footer with contact & quick links

### Page Components
- Hero w/ CTA
- Grid card layout for products
- Service icons + blurbs
- About preview section
- Testimonial or CTA banner
- Admin dashboard form inputs

---

## 🧾 Asset Expectations
Use the logo. Everything else (icons, images, colors) must be generated or sourced according to:
- Blue/white/yellow palette
- Light industrial look
- Home improvement visuals (gutters, roofs, aluminum, etc.)

---

## 🔐 Admin Functionality
- Firebase email login
- Admin-only access to CRUD dashboard
- Firestore schema: `products`, `services`, `articles`, `users`
- Firestore rules: no write access for public users

---

## ✅ MVP Must-Haves
- Fully functional product catalog w/ admin CRUD
- Mobile-first layout using Tailwind
- Nav + footer
- 4-5 essential pages (Home, Products, Services, About, Contact)
- Firebase Auth + Firestore hooked up and deployed

---

## 🧠 Agent Behavior
When unsure:
- Ask the user to clarify
- Offer multiple design/code options
- Prioritize code reuse and DRY principles
- Keep responses short and useful
- Be professional, but chill and human
