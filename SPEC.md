# Design handoff spec · v2

**Figma file:** Screens: see the published link (HTML, not Figma)
**Final page:** Screens: see the published link (HTML, not Figma)

## Screens

| # | Screen | Language | Frame name | Priority |
| --- | --- | --- | --- | --- |
| 1 | Customer Address Entry | English | customer_entry.html | must |
| 2 | Rider Order View | Korean | rider_view.html | must |

## English input → Korean display

| Customer enters (English screen) | Field name (Data Guide) | Rider sees (Korean screen) | Notes |
| --- | --- | --- | --- |
| Delivery Address | road_address_en | road_address_ko | Main address block |
| Detail Address | building_name_en | building_name_ko | Secondary building line |
| Delivery Note | delivery_note | delivery_note | Customer requests card |

## States per screen

| Screen | Default | Empty | Error | Other (loading, no results) |
| --- | --- | --- | --- | --- |
| Customer Entry | Address and note filled | Blank inputs with placeholder | Invalid address inline error | Address searching indicator |
| Rider Order View | Korean address and note card | Missing address fallback text | Failed to load order details | Loading order details |

## Specs

- **Spacing:** use the value from the design guide
- **Colors:** use the value from the design guide
- **Type:** use the value from the design guide
- **Components:** Text input, text area, button, order card (states: default, focused, error, disabled)
- Mobile frame size: 390 × 844

## Assets

- Export CSS and inline SVG icons

## Open decisions

- None

## Changes since the last version

- Realigned scope from animal designs to customer address entry and rider order view screens per developer feedback.