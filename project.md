Atlantic Gutter Supply Website Redesign - MVP Task Outline

⸻

Overview

This document outlines the minimum viable product (MVP) features and development tasks required to launch the redesigned Atlantic Gutter Supply website. The goal is to create a modern, responsive, and functional site that supports product catalog CRUD operations, improved information architecture, and a professional design aligned with the new branding.

⸻

MVP Goals
	•	Modern and mobile-friendly redesign using updated logo and color scheme
	•	Clean, intuitive UI with strong CTA hierarchy
	•	Informational pages for services, products, company, and contact
	•	Dynamic product catalog with create/read/update/delete (CRUD) capabilities
	•	Admin authentication and protected admin panel
	•	Easy-to-maintain content structure

⸻

Technical Stack
	•	Frontend: SvelteKit + Tailwind CSS v4
	•	Backend: Firebase (Firestore for data, Auth for login)
	•	Storage: Firebase Storage or Cloudinary for product images
	•	Hosting: Vercel

⸻

Pages to Build
	1.	Homepage
	•	Hero section with CTA
	•	Value propositions
	•	About preview
	•	Service preview
	•	Product preview
	•	Knowledge base teaser
	•	Footer
	2.	Products Page
	•	Grid layout with filters (K Style, Half Round, Euro, etc)
	•	Product detail pages
	3.	Services Page
	•	Delivery fleet
	•	Tooling
	•	Gutter machine repair
	•	Consultation and pricing
	4.	About Us Page
	•	Company history
	•	Mission, values, team
	5.	Knowledge Base (optional MVP)
	•	Article list and single post view
	6.	Contact Page
	•	Contact form
	•	Google Maps embed
	•	Business hours and info
	7.	Admin Panel (Protected Route)
	•	Login via Firebase Auth
	•	Product CRUD interface
	•	Optional service/blog post management

⸻

Tasks

Design & Assets
	•	Finalize color palette & typography
	•	Generate favicon
	•	Source stock or in-house photos for hero, products, background, etc.
	•	Generate icons for services/values

Frontend
	•	Set up SvelteKit project with Tailwind
	•	Create layout shell with nav/footer
	•	Build each page template
	•	Create components for reusable sections (hero, cards, CTAs, etc.)

Backend
	•	Set up Firebase project
	•	Configure Firestore collections (products, users, etc.)
	•	Configure Firebase Auth (email/password login)
	•	Build protected admin panel routes
	•	Implement CRUD operations

QA & Deployment
	•	Responsive testing
	•	Cross-browser testing
	•	SEO basic meta tags and accessibility
	•	Deploy to Vercel or Netlify

⸻

Asset Checklist

Provided

To Generate
	•	Logo (SVG/PNG)
	•	Favicon (32x32 PNG)
	•	Color palette and font pairing reference
	•	Hero section image (gutter installation or abstract water/rain texture)
	•	Background textures (e.g. metal, industrial, or paper)
	•	Product photos (placeholder or actual, both thumbnail and full size)
	•	Stock/in-house imagery of delivery fleet, warehouse, tooling, etc.
	•	Icons for:
	•	Material
	•	Appearance
	•	Functionality
	•	Installation
	•	Delivery
	•	Tooling
	•	Pricing
	•	Team photo or workspace photo (for About page)
	•	Testimonial image (optional)
	•	Knowledge base/blog header image (optional)

Generated
	•	Favicon (32x32 PNG)
	•	Color palette and font pairing reference
	•	Icons for services/values

⸻

Post-MVP Ideas
	•	Knowledge base or blog system
	•	Live inventory or price updates
	•	Customer testimonials carousel
	•	Email capture/newsletter
	•	Social media integration

⸻
