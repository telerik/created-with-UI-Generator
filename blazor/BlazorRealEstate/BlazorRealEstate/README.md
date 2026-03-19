# BlazorRealEstate

A Blazor Web App featuring a real estate property search page built with [Telerik UI for Blazor](https://www.telerik.com/blazor-ui).

## About the Prompt

The real estate search page was generated using a GitHub Copilot agent prompt located at:

```
.github/prompts/real-estate-search-page.prompt.md
```

This is a `.prompt.md` file — a reusable prompt that can be run directly in VS Code via the **GitHub Copilot Chat** panel. Open it in the editor, type `/real-estate-search-page`, and the agent will execute the prompt, generating the entire page in one go. The prompt includes detailed instructions for the UI layout, filter options, and property result cards, ensuring a comprehensive real estate search experience.

## What the Prompt Builds

Running the prompt generates the complete real estate search page in `BlazorRealEstate/Components/Pages/Home.razor`. The page includes:

### Filter Sidebar
- **Keyword search** — free-text `TelerikTextBox` for terms like "pool" or "open floor plan"
- **Location** — city, ZIP, or neighborhood search
- **Price range** — `TelerikRangeSlider` with $10 k increments, formatted labels, no tick marks
- **Property type** — multi-select `TelerikChipList` (House, Condo, Townhouse, etc.)
- **Bedrooms / Bathrooms** — range sliders
- **Square footage / Lot size** — range sliders
- **Year built** — range slider
- **Amenities** — collapsible panel with checkboxes (pool, garage, fireplace, etc.)

### Property Results
- Cards showing a placeholder image (via **Unsplash**), bold title, address, SqFt, bedroom and bathroom icons
- Sort menu: **Best Match**, **Top Selling**, **Price** (ascending/descending toggle)

### Responsive Layout
- **Desktop** — golden-ratio split: filter sidebar on the left, results on the right
- **Mobile** — stacked layout with a show/hide toggle button for the filter panel

## Running the Project

```bash
dotnet run --project BlazorRealEstate/BlazorRealEstate.csproj
```

Navigate to `https://localhost:<port>` to see the home page with the real estate search UI.
