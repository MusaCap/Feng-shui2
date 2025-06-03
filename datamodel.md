# 🗂️ FengShuiFlow – Data Model

This data model defines the key entities, relationships, and attributes for the FengShuiFlow application. It supports room layout scanning, object detection, Feng Shui analysis, and personalized furniture arrangement recommendations.

---

## 1. Entity: `User`

| Field         | Type     | Description                          |
|---------------|----------|--------------------------------------|
| user_id       | UUID     | Unique identifier for the user       |
| email         | String   | User email address                   |
| name          | String   | Full name                            |
| preferences   | JSON     | Layout goals, energy focuses, style  |
| created_at    | DateTime | Account creation timestamp           |
| last_login    | DateTime | Last activity timestamp              |

---

## 2. Entity: `Room`

| Field         | Type     | Description                          |
|---------------|----------|--------------------------------------|
| room_id       | UUID     | Unique identifier for the room       |
| user_id       | UUID     | Reference to the user                |
| name          | String   | "Living Room", "Bedroom", etc.       |
| dimensions    | JSON     | Length, width, height (in meters/ft) |
| floor_plan    | Image/URL| Uploaded blueprint or scanned layout |
| bagua_map     | JSON     | Bagua zone overlay (coordinates + zone) |
| created_at    | DateTime | Room created timestamp               |

---

## 3. Entity: `FurnitureItem`

| Field         | Type     | Description                            |
|---------------|----------|----------------------------------------|
| item_id       | UUID     | Unique ID for the furniture item       |
| room_id       | UUID     | Reference to the room                  |
| name          | String   | Name/label (e.g., "Sofa", "Desk")      |
| type          | String   | Category (e.g., seating, storage)      |
| dimensions    | JSON     | Length, width, height                  |
| position      | JSON     | X, Y coordinates in the room layout    |
| rotation      | Float    | Angle/orientation                      |
| material      | String   | Primary material (wood, metal, etc.)   |
| element       | String   | Feng Shui element (wood, fire, etc.)   |
| is_fixed      | Boolean  | Whether the item can be moved          |
| sentimental   | Boolean  | Whether to preserve location/value     |

---

## 4. Entity: `FengShuiAnalysis`

| Field             | Type     | Description                              |
|------------------|----------|------------------------------------------|
| analysis_id       | UUID     | Unique ID                                |
| room_id           | UUID     | Associated room                          |
| energy_score      | Integer  | Harmony score (0–100)                    |
| blocked_zones     | JSON     | List of zones with obstructions          |
| recommendations   | JSON     | Textual + spatial suggestions            |
| suggested_layouts | JSON     | 2D/3D furniture arrangements             |
| goal              | String   | Optimization intent (e.g., career, love) |
| created_at        | DateTime | Timestamp of analysis                    |

---

## 5. Entity: `RetailFurnitureOption`

| Field         | Type     | Description                                |
|---------------|----------|--------------------------------------------|
| retail_id     | UUID     | Unique identifier                          |
| item_name     | String   | Name of retail furniture                   |
| vendor        | String   | Retailer name (e.g., IKEA, Wayfair)        |
| product_url   | String   | Link to purchase page                      |
| image_url     | String   | Product image                              |
| dimensions    | JSON     | Dimensions for compatibility               |
| fengshui_tags | JSON     | Element type, placement suitability        |
| price         | Float    | Cost in user's preferred currency          |

---

## 6. Relationships

```plaintext
User          1 — * Room
Room          1 — * FurnitureItem
Room          1 — * FengShuiAnalysis
FurnitureItem * — * RetailFurnitureOption (via suggestions)
