---
name: real-estate-search-page
description: Build a real estate listing page that includes a dedicated Filter UI section.
agent: agent
model: Claude Sonnet 4.6 (copilot)
tools: [execute, read, edit, search, web, agent, todo, telerik-blazor-mcp/*]
---

<!-- 
estimated-human-time: 2 hours
estimated-ai-time: 10:28 minutes:seconds
-->

# Instructions

Build a real estate listing page that includes a dedicated Filter UI section. The filter area should be visually separated from the main property results as a sidebar. Filters must be contextual to real estate inventory.

## Page Layout

### Desktop Layout (golden ratio)

| Filter UI | Filter Results |

### Mobile

[ Filter UI (hide/show)]

[ Filtered Results ]

## Filter UI Instructions
Include filters commonly used in real estate searches, such as price range, number of bedrooms and bathrooms, property type, square footage, lot size, year built, amenities, and location. The UI should help users refine listings quickly and discover properties that match their needs.

- Keyword search: Textbox
- Range sliders should hide graduation marks and format in 10k increments.
- Amenities: Show in a collapsible panel and use checkboxes
- Property Type: Multiple selection with chip UI

## Filtered Results Instructions

Show cards for each available unit: Image, Title (large and bold), address, square footage (SqFt), bedrooms (icon) #, bath (icon) #. Each card should have an image (use images.unsplash.com as placeholders).

Display a sort menu at the top of the view. [Best match | Top Selling | Price (up/down toggle)]