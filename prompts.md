## Prompt Design

### Outfit Generation Prompt (Simplified)

Generate three independent outfit options based on:

Context:
- Weather
- Occasion
- Gender
- Style preference

Constraints:
- Only use selected wardrobe items
- Must include:
  - Top
  - Bottom (unless dress)
  - Shoes
- Avoid items excluded by user
- Ensure diversity across options
- Provide explanation for each outfit

---

### Keyword Handling

Examples:

User input | System behavior
--- | ---
no jeans | remove jeans
no pants | remove pants
not rain | remove rain-related items
formal | increase formality level
comfortable | prioritize relaxed fit

Negative constraints override defaults.

---

### Diversity Control

- Generate each option independently
- Regeneration affects only selected option
- Avoid repeating same bottom/shoes across all options
