# CardServices

A flexible section component that showcases six company services with terminal-themed dashboards. Each service has a dedicated variant with customizable content and metrics display.

## Overview

CardServices displays a collection of automation services with an interactive variant switcher. Each of the six services is represented by a variant that contains an embedded TerminalDashboard for detailed metrics and information.

![CardServices](/images/guide/synthexa-77@2x.png)

**Key Features:**
- Six service variants (01–06) for different automation offerings
- Section title, description, and Desktop/Mobile toggle
- Integrated TerminalDashboard in each variant
- Customizable spacing and padding
- Prefix and section label configuration

## How to Edit

### Select the Component

To customize CardServices properties:

1. **Select the component** — Click CardServices directly on the canvas, OR find it in the **Layers** panel and click its name
2. **Open Properties** — The Properties panel (right sidebar) displays all section-level properties
3. **Make changes** — Edit properties and see changes update in real-time

### Edit Individual Service Variants

To customize the TerminalDashboard inside each service variant:

1. Click **Edit Component** button at the bottom of Properties
2. You'll see all 6 service variants (buttons 01–06)
3. Click the variant button to switch between services
4. Click on the TerminalDashboard inside the selected variant
5. Edit its properties (metrics, colors, panel layout, etc.)
6. Refer to [TerminalDashboard documentation](/synthexa/components/terminal) for all available properties

## Property Controls

### Content

| Property | Type | Default | Description |
|----------|------|---------|-------------|
| **Variant** | Dropdown | 01 | Select which service variant to display (01–06) |
| **Title** | String | "From manual workflows to auto..." | Section heading displayed above the service content |
| **Description** | String | "We design and build workflows..." | Detailed explanation of the services |
| **Desktop** | Toggle | Yes / No | Controls whether the service displays on desktop or mobile layout |

### Section Structure

| Property | Type | Default | Description |
|----------|------|---------|-------------|
| **Prefix** | String | "//" | Visual prefix before the section label (e.g., "//") |
| **Section Label** | String | "workflows" | Label text displayed in the section header |

### Spacing

| Property | Type | Default | Description |
|----------|------|---------|-------------|
| **Gap** | Spacing | 64px X, 64px Y | Space between main section elements (horizontal and vertical) |
| **Gap 2** | Number | 32px | Secondary spacing between nested elements |
| **Padding** | Spacing | 0 (all sides) | Inner padding around the entire component (Top, Right, Bottom, Left) |

## Variants Explained

The CardServices component includes six pre-configured service variants:

| Variant | Use Case |
|---------|----------|
| **01** | First automation service offering |
| **02** | Second automation service offering |
| **03** | Third automation service offering |
| **04** | Fourth automation service offering |
| **05** | Fifth automation service offering |
| **06** | Sixth automation service offering |

Each variant displays the same structure with a TerminalDashboard that shows service-specific metrics and details.

## Customizing Service Details

Each service variant contains a TerminalDashboard with:
- **Metrics panels** — Key performance indicators
- **Terminal output** — Service description and automation details
- **Color scheme** — Terminal Primary/Secondary colors for consistency
- **Custom SVG** — Charts or diagrams specific to the service

To edit these elements:

1. Click **Edit Component** in the Properties panel
2. Select the service variant (01–06)
3. Click on elements inside the TerminalDashboard
4. Refer to [TerminalDashboard documentation](/synthexa/components/terminal) for detailed customization options

## Best Practices

- **Consistency** — Keep all six services visually aligned with matching spacing
- **Metrics** — Use consistent units and formatting across all services (e.g., "~2 hrs saved", "$4,800 ROI")
- **Descriptions** — Keep service descriptions concise and benefit-focused
- **Desktop Toggle** — Use the Desktop property to control layout responsiveness
- **Section Label** — Keep the section label short and descriptive (e.g., "workflows", "automations")

## Next Steps

→ [CardPattern](/synthexa/components/card-pattern)

→ [TerminalDashboard](/synthexa/components/terminal)

→ [Other Components](/synthexa/components/other)
