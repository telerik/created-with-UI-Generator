# BlazorRealEstate

A Blazor Web App featuring a real estate property search page built with [Telerik UI for Blazor](https://www.telerik.com/blazor-ui).

## Video

[![Watch the video](https://img.youtube.com/vi/jUho9Jy_Qy4/0.jpg)](https://www.youtube.com/embed/jUho9Jy_Qy4?si=d5OxhszltkhEHyMx)

<iframe width="560" height="315" src="" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## About the Prompt

The real estate search page was generated using a GitHub Copilot agent prompt located at:

```
.github/prompts/real-estate-search-page.prompt.md
```

This is a `.prompt.md` file — a reusable prompt that can be run directly in VS Code via the **GitHub Copilot Chat** panel. Open it in the editor, type `/real-estate-search-page`, and the agent will execute the prompt, generating the entire page in one go. The prompt includes detailed instructions for the UI layout, filter options, and property result cards, ensuring a comprehensive real estate search experience.

## Time Savings

Using this prompt with the Telerik UI Generator saves an estimated **2 hours** compared to manually building the same page from scratch. The agent handles all the component selection, layout design, and code generation, allowing you to focus on customizing and enhancing the UI rather than writing boilerplate code.

Total build time with the prompt: **10 minutes** (including review and minor adjustments)

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
