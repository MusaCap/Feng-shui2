# 🗓️ FengShuiFlow Sprint Plan (For Windsurf AI Agent System)

## 🏁 Sprint Duration
- **2 weeks per sprint**
- **8 total sprints (16 weeks MVP)**
- 3-person squad (Frontend, Backend, AI/AR Engineer)

---

## 🚀 Sprint 1: Foundation & Onboarding (Week 1–2)

### Objectives:
- Stand up auth system
- Define initial data models
- Begin onboarding UX

### Tasks:
- [ ] US001 – Email/password + SSO (Google/Apple)
- [ ] US002 – Create onboarding screen (layout intent + Feng Shui goals)
- [ ] US003 – Build and test `User`, `Room`, and `FurnitureItem` schemas
- [ ] US005 – Add welcome tutorial

**Deliverables:**  
✅ Auth, database schema, onboarding flow MVP

---

## 🚧 Sprint 2: Room Input (Manual + Upload) (Week 3–4)

### Objectives:
- Room layout via drawing or blueprint
- Start Bagua mapping logic

### Tasks:
- [ ] US010 – Upload blueprint/floorplan
- [ ] US011 – Manual room drawing tool (canvas UI)
- [ ] US014 – Room labeling (type, name)
- [ ] US030 – Initial Bagua map overlay logic

**Deliverables:**  
✅ Upload & draw layout capability with Bagua preview

---

## 🧠 Sprint 3: Furniture Input & Tagging (Week 5–6)

### Objectives:
- Add furniture items manually or via AR
- Enable object tagging and spatial metadata

### Tasks:
- [ ] US020 – Add furniture from library
- [ ] US021 – Integrate AR scanning (ARKit/ARCore)
- [ ] US022 – Save position, material, and dimensions
- [ ] US023 – Enable "sentimental" and "immovable" tags

**Deliverables:**  
✅ Room + furniture scene setup complete with metadata capture

---

## 🔮 Sprint 4: Feng Shui Engine v1 (Week 7–8)

### Objectives:
- Harmony score calculation
- Optimize based on Bagua violations

### Tasks:
- [ ] US031 – Detect blocked energy zones
- [ ] US032 – Calculate harmony score (0–100)
- [ ] US033 – Recommend layout based on energy goal
- [ ] US034 – Provide reasoning per suggestion

**Deliverables:**  
✅ First-pass Feng Shui suggestions & scoring engine

---

## 🧩 Sprint 5: Layout Visualization (Week 9–10)

### Objectives:
- Introduce 2D/3D layout preview
- Allow layout toggles and edits

### Tasks:
- [ ] US040 – Build 2D top-down editor
- [ ] US041 – Generate 3D view (Three.js or Unity WebGL)
- [ ] US044 – Save layouts per room version
- [ ] US043 – Enable before/after comparison

**Deliverables:**  
✅ Visual layout manipulation + energy improvement feedback loop

---

## 🛍️ Sprint 6: Retail Integration & Suggestions (Week 11–12)

### Objectives:
- Add e-commerce suggestion layer
- Connect layouts to real products

### Tasks:
- [ ] US050 – Ingest retail catalogs (IKEA, Wayfair mock data)
- [ ] US051 – Match by dimensions + Feng Shui element
- [ ] US052 – Embed "Buy Now" links in UI
- [ ] US053 – Add price range filter

**Deliverables:**  
✅ Layout-to-product pipeline functioning with real furniture

---

## 🧘 Sprint 7: Sharing, Export, and Feedback (Week 13–14)

### Objectives:
- Empower sharing and improvement reflection

### Tasks:
- [ ] US060 – Export PDF with energy report
- [ ] US061 – Shareable link generation (private/public)
- [ ] US062 – Pinterest / Instagram export
- [ ] US073 – Log user feedback on layouts

**Deliverables:**  
✅ Export + social-ready layout sharing with reflection feedback

---

## 🌐 Sprint 8: Polish, Premium, and Launch Prep (Week 15–16)

### Objectives:
- Add basic monetization
- Optimize UX and prep deployment

### Tasks:
- [ ] US080 – Add premium layout options (e.g., by goal)
- [ ] US081 – GPT-based Feng Shui AI coach (basic prompt config)
- [ ] US092 – Final accessibility sweep (WCAG compliance)
- [ ] US070 – Build lightweight admin analytics dashboard

**Deliverables:**  
✅ Monetization hooks, coach assistant, admin QA tools

---

## 🏁 Final MVP Delivery Criteria

- Functional across mobile and web
- At least 1 room → 1 furniture layout → 1 energy score improvement cycle
- Export, share, and receive at least 1 layout suggestion
- AR input (basic) and Bagua overlay functioning

---

## 🗂️ Windsurf Project Tags

```yaml
project:
  name: FengShuiFlow
  category: lifestyle, interior, AI, AR
  agents: ['frontend-dev', 'backend-dev', 'ar-ai-specialist']
  tools: ['Flutter', 'React', 'Firebase', 'FastAPI', 'Three.js', 'ARKit', 'GPT-4']
