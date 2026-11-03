# Student Cafe

HCI Lab 07: Figma design converted to a responsive HTML5 website with Tailwind CSS.

## Links

- Figma design: <https://www.figma.com/design/W1UgyDcP2UChvqSnukkJ1L/Studend-Cafe?node-id=9-2>
- Live site: `PASTE YOUR GITHUB PAGES URL HERE`

## Figma MCP Setup

The VS Code MCP configuration is stored in `.vscode/mcp.json`:

```json
{
  "servers": {
    "figma": {
      "type": "http",
      "url": "https://mcp.figma.com/mcp"
    }
  }
}
```

The design was inspected with the Figma MCP server using the `PageDesktop` frame (`9:2`).

## Design tokens extracted from Figma

| Category | Tokens |
|---|---|
| Colors | primary `#235d3a`; text `#243b2e`; text-muted `#526457`; surface `#ffffff`; border `#d6ded6`; background `#fff9f1`; on-primary `#ffffff` |
| Spacing | `0`, `8`, `12`, `16`, `24`, `32`, `64`, `160` px |
| Font sizes | small `14px`; body `16px`; body-large `18px`; card-title `24px`; section-title `32px`; hero-title `48px` |
| Line heights | `20px`, `24px`, `28px`, `32px`, `40px`, `56px` |
| Border radius | `0px`, `8px`, `16px`, `24px` |
| Font family | Arimo |

These values are defined as CSS custom properties in `index.html` and mapped into the Tailwind CDN configuration.

## Tools and structure

- Figma MCP server configured in `.vscode/mcp.json`
- HTML5 landmarks: header, nav, main, section, footer
- Tailwind CSS loaded from CDN
- Sections: navigation, hero, campus favourites, contact form, footer

## Responsiveness and accessibility

- Viewports tested: 1440px, 768px, and 375px
- No horizontal scrolling at the tested viewport sizes
- Cards use 3 columns on large screens, 2 on medium screens, and 1 on mobile
- Visible hover and focus-visible states
- Labels are bound to form controls
- The hero image has descriptive alt text
- Menu and Contact navigation links target their corresponding sections
