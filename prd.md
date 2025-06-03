# 🧾 Product Requirements Document (PRD)

## Product Name  
**FengShuiFlow – Home Energy Organizer**

## Author  
Product Team, Musa Capital

## Date  
June 3, 2025

---

## 1. Purpose

To create a mobile and web-based application that helps users organize furniture and décor in their home according to Feng Shui principles. The application will take a room layout (via scan, blueprint upload, or manual input) and generate optimized furniture arrangements that improve energy flow, harmony, and functionality.

---

## 2. Background & Motivation

Modern urban living often leads to disorganized or poorly arranged furniture that can impact mood, productivity, and wellness. Feng Shui is an ancient Chinese practice that promotes harmony through spatial arrangement and energy balance. This app leverages traditional Feng Shui rules, modern AI, and spatial recognition to help users harmonize their homes with minimal effort.

---

## 3. Key Features

### 🔍 Room Input & Scanning
- Upload blueprints or manually draw room layout.
- Use phone camera (AR) to scan room dimensions.
- Detect windows, doors, and fixed furniture (e.g. kitchen cabinets).

### 🧭 Feng Shui Analyzer
- Identify Bagua map zones overlaid on room layout.
- Detect energy flow blockages.
- Classify objects by elemental influence (wood, water, fire, metal, earth).

### 🪑 Smart Layout Suggestions
- AI-powered furniture reconfiguration proposals.
- Multiple layout options: career-focused, health-enhancing, wealth-attracting, etc.
- Interactive 2D and 3D previews.
- "Move this here" guided reconfiguration view using AR.

### 📦 Furniture Database
- Sync with common furniture stores (IKEA, Wayfair).
- Suggest Feng Shui-friendly replacements if items violate principles.
- Option to tag items with sentimental or inherited value to preserve.

### 🧘 Energy Score
- Feng Shui harmony score (0–100 scale).
- Real-time updates as changes are made.
- Personalized suggestions to improve score.

### 🔄 Sharing & Export
- Save, export, or share designs.
- Generate before/after comparison.
- Integration with Pinterest and Instagram.

---

## 4. User Stories

| As a...         | I want to...                              | So that...                                 |
|----------------|-------------------------------------------|--------------------------------------------|
| Homeowner      | Scan my living room                       | I can get personalized Feng Shui layout suggestions |
| Interior designer | Upload floor plans                    | I can generate client layouts based on Feng Shui |
| Renter         | Get recommendations without moving heavy items | I can optimize my space without major effort |
| Enthusiast     | Learn about energy zones                 | I can apply Feng Shui intentionally        |

---

## 5. User Flow

1. Onboard → Choose room type → Scan/upload layout  
2. Detect furniture → Overlay Bagua map → View energy analysis  
3. Select desired energy goal (e.g., better sleep, more abundance)  
4. View optimized layouts → Accept and export or tweak  
5. Get final layout + score → Option to purchase suggested items

---

## 6. Technical Requirements

### Platform
- iOS, Android (Flutter)
- Web (React)

### Backend
- Firebase (auth, storage)
- Python + FastAPI (Feng Shui logic engine)
- PostGIS / spatial database

### 3D/AR
- ARKit (iOS), ARCore (Android)
- Three.js or Unity WebGL (web viewer)

---

## 7. Non-Functional Requirements

- Privacy compliant (GDPR, CCPA)
- Fast rendering (<1s for layout switch)
- Offline mode for viewing saved layouts
- Accessible UI/UX (WCAG 2.1 AA)

---

## 8. Success Metrics

- User NPS > 60
- Weekly active users (WAU) > 10,000
- >40% of users complete layout optimization in first session
- Integration with at least 3 furniture retailers in first year

---

## 9. Future Features (Backlog)

- Feng Shui coaching chat agent
- VR room walkthrough
- Multi-room optimization
- Seasonal rebalancing suggestions
- Cultural adaptations (Vastu, Wabi-Sabi)
