# Design handoff spec · Address Entry and Rider View · v2

**Figma file:** Screens: see the published link (HTML, not Figma)
**Final page:** Screens: see the published link (HTML, not Figma)

## Screens

| # | Screen | Language | Frame name | Priority |
| --- | --- | --- | --- | --- |
| 1 | Address entry | English | address.html | must |
| 2 | Rider order detail | Korean | rider.html | must |

## English input → Korean display

| Customer enters (English screen) | Field name (Data Guide) | Rider sees (Korean screen) | Notes |
| --- | --- | --- | --- |
| Street address search | road_address_en | road_address_ko | Translated road address shown prominently |
| Building name | building_name_en | building_name_ko | Korean building name display |
| Detail address (e.g. Room 101) | detail_address | 동/호수 정보 | Key location detail |
| Delivery notes | delivery_note | 배달 요청사항 | Displayed in Korean for rider clarity |

## States per screen

| Screen | Default | Empty | Error | Other (loading, no results) |
| --- | --- | --- | --- | --- |
| address.html | Address fields filled with initial values | Clean inputs with placeholder text | Red highlight on invalid address field | Address search loading indicator |
| rider.html | Translated Korean address and delivery notes | Message showing no active delivery order | Network error state message | Loading order data |

## Specs

- **Spacing:** use the value from the design guide
- **Colors:** use the value from the design guide for text, background, primary, error
- **Type:** use the value from the design guide
- **Components:** Text inputs (default, focused, error), Primary action button, Information cards
- Mobile frame size: 390 × 844

## Assets

- Export: Inline SVG icons and shared CSS tokens
- Where: Relative CSS file (styles.css)

## Open decisions

- [none]

## Changes since the last version

- Updated design spec and HTML screens to focus strictly on English customer entry and Korean rider view flows.