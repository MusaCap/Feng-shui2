# 🧰 FengShuiFlow – Full Backlog (for Windsurf Execution)

## Epic 1: User Onboarding & Authentication
### Goal: Let users sign up, log in, and define their layout goals

- [ ] **US001** – Implement user registration (email + password)
- [ ] **US002** – Enable Google and Apple SSO
- [ ] **US003** – Create onboarding flow to select layout intent (e.g., “better sleep”, “more prosperity”)
- [ ] **US004** – Store user preferences and Feng Shui familiarity level
- [ ] **US005** – Add welcome tutorial and skip option

---

## Epic 2: Room Input (Blueprint / Manual / AR)
### Goal: Enable users to input room dimensions via multiple methods

- [ ] **US010** – Allow upload of image/PDF floor plans
- [ ] **US011** – Enable manual room drawing with drag-to-size interface
- [ ] **US012** – Integrate AR room scanner (ARKit/ARCore)
- [ ] **US013** – Auto-detect room boundaries, windows, and doors from scan
- [ ] **US014** – Provide room labeling and room type tagging

---

## Epic 3: Furniture Detection & Tagging
### Goal: Populate furniture layout and classify items

- [ ] **US020** – Manually add furniture (drag and drop library)
- [ ] **US021** – Enable AR-based object recognition and size capture
- [ ] **US022** – Store object metadata (type, size, material)
- [ ] **US023** – Allow user tagging: "Sentimental", "Unmovable", "Decorative"
- [ ] **US024** – Classify furniture by Feng Shui element

---

## Epic 4: Feng Shui Engine & Layout Optimizer
### Goal: Provide energy analysis and layout improvement suggestions

- [ ] **US030** – Overlay Bagua map to floor plan with calibration controls
- [ ] **US031** – Identify blocked energy zones and list violations
- [ ] **US032** – Score layout on harmony scale (0–100)
- [ ] **US033** – Generate optimized layouts based on user goal (e.g., love, wealth, creativity)
- [ ] **US034** – Suggest multiple layout versions with user feedback loop
- [ ] **US035** – Explain reasoning per layout suggestion (text + visuals)

---

## Epic 5: 2D/3D/AR Layout Rendering
### Goal: Display optimized room setups visually and immersively

- [ ] **US040** – Build 2D layout view with drag-and-drop customization
- [ ] **US041** – Generate 3D layout rendering using Three.js or Unity WebGL
- [ ] **US042** – Add AR placement preview with step-by-step guidance
- [ ] **US043** – Toggle between before/after views
- [ ] **US044** – Save multiple layout versions per room

---

## Epic 6: Retail Integration & Suggestions
### Goal: Help users buy compatible Feng Shui-friendly items

- [ ] **US050** – Build retail catalog ingestion (IKEA, Wayfair, etc.)
- [ ] **US051** – Match replacement items to Feng Shui element and size constraints
- [ ] **US052** – Provide "Buy Now" links from layout view
- [ ] **US053** – Enable user preference toggles for budget, style, retailer

---

## Epic 7: Social & Export Features
### Goal: Let users share, export, and reflect on improvements

- [ ] **US060** – Export layout as PDF with energy report
- [ ] **US061** – Enable layout sharing via link (public/private setting)
- [ ] **US062** – Add Pinterest, Instagram, and TikTok export integration
- [ ] **US063** – Auto-generate side-by-side before/after images

---

## Epic 8: Admin, Analytics & Backend
### Goal: Enable backend support, tracking, and analytics

- [ ] **US070** – Admin dashboard for bug tracking and content moderation
- [ ] **US071** – Store layout analytics per user (energy score deltas, items moved)
- [ ] **US072** – Track engagement metrics (layout completion rate, AR usage)
- [ ] **US073** – Log feedback on layout quality and usefulness

---

## Epic 9: Premium Features & Subscription
### Goal: Introduce monetization with value-added tools

- [ ] **US080** – Gated layout types and advanced Bagua overlays
- [ ] **US081** – Feng Shui coach AI chat assistant (GPT-4-based)
- [ ] **US082** – Seasonal rebalance notifications (e.g., Spring Equinox update)
- [ ] **US083** – Payment system integration (Stripe, Apple Pay)

---

## Epic 10: Localization, Accessibility, & Culture
### Goal: Expand app for diverse audiences and usability

- [ ] **US090** – Translate app to Mandarin, Spanish, and Hindi
- [ ] **US091** – Add Vastu Shastra and Wabi-Sabi mode for non-Chinese users
- [ ] **US092** – Ensure full accessibility (WCAG 2.1 AA compliance)
- [ ] **US093** – Support imperial/metric toggle

---

## 🧭 Backlog Tagging for Windsurf

```yaml
tags:
  - frontend
  - backend
  - ar
  - ai
  - retail
  - localization
  - monetization
  - accessibility
  - ux
  - analytics
