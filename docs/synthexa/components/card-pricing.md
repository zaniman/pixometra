# CardPricing & PricingPlans

A comprehensive pricing section component that displays tiered pricing plans with monthly/yearly toggle, customizable features, and responsive variants for desktop and mobile.

## Overview

**PricingPlans** is the main section component that includes:
- Section header with title and description
- Monthly/Yearly toggle switch
- Three pricing plan cards (Plan1, Plan2, Plan3)
- Responsive variants for desktop and mobile

**CardPricing** is an individual pricing plan card with:
- Plan name and description
- Monthly and yearly pricing
- Feature list with inclusion indicators
- CTA button with custom label and icon
- Link to contact or signup page

## How to Edit

### Edit Section-Level Properties

To customize the pricing section header and layout:

1. **Select PricingPlans** on the canvas OR in the **Layers** panel
2. **Open Properties** — The Properties panel displays section settings
3. **Edit properties:**
   - **Prefix** — Visual prefix (e.g., "//")
   - **Section Label** — Section name (e.g., "pricing")
   - **Title** — Main heading (e.g., "Start saving this month")
   - **Description** — Section subtitle
   - **Background Pattern** — Toggle background pattern visibility
   - **Variant** — Switch between Yearly/Monthly/YearlyMobile/MonthlyMobile

### Edit with Edit Component

To access all section variants:

1. Click PricingPlans to select it
2. Click **Edit Component** button in Properties
3. You'll see 4 variants:
   - **Yearly** (Primary) — Desktop yearly view
   - **Monthly** — Desktop monthly view
   - **YearlyMobile** — Mobile yearly view
   - **MonthlyMobile** — Mobile monthly view

**Important:** Always make pricing changes in the **Yearly | Primary** variant. Changes automatically apply to all other variants.

## Property Controls

### Section Level (PricingPlans)

| Property | Type | Default | Description |
|----------|------|---------|-------------|
| **Prefix** | String | "//" | Visual prefix before section label |
| **Section Label** | String | "pricing" | Section identifier text |
| **Title** | String | "Start saving this month" | Main section heading |
| **Description** | String | "Choose a setup that fits..." | Subtitle describing pricing |
| **Background Pattern** | Toggle | Yes | Show background pattern |
| **Variant** | Dropdown | Yearly | Select which variant to display (Yearly / Monthly / YearlyMobile / MonthlyMobile) |

### Card Level (CardPricing)

| Property | Type | Description |
|----------|------|-------------|
| **Variant** | Dropdown | Select Yearly or Monthly pricing display |
| **Title** | String | Plan name (e.g., "Starter", "Growth", "Custom") |
| **Description** | String | Brief plan description |
| **Monthly Price** | Number | Price for monthly billing (slider input) |
| **Monthly Text** | String | Label below monthly price (e.g., "/ month") |
| **Yearly Price** | Number | Price for yearly billing (slider input) |
| **Yearly Text** | String | Label below yearly price (e.g., "/ month, billed annually") |
| **Button** | Dropdown | Button style (Primary / Secondary) |
| **Button Label** | String | CTA text (e.g., "Start automating", "Talk to us") |
| **Button Icon** | Icon | Icon displayed in button (e.g., "Arrow Right") |
| **Features 1-5** | String | Feature names (e.g., "Automate up to 3 workflows") |
| **Feature 1-5 Included** | Dropdown | Enabled / Disabled (show checkmark or X) |
| **Elevated Background** | Toggle | Add subtle background highlight |
| **Link** | URL | Button link destination (e.g., "/contact") |

## Editing Pricing Cards

### Update Plan Information

To edit Plan1, Plan2, or Plan3:

1. **Important:** Always edit in the **Yearly | Primary** variant first
2. Click on the plan card (or select Plan1/Plan2/Plan3 in **Layers**)
3. In **Properties**, update:
   - **Title** — Plan name
   - **Description** — Plan description
   - **Monthly Price** / **Yearly Price** — Adjust with slider or type number
   - **Monthly Text** / **Yearly Text** — Price period text
   - **Button Label** — CTA text
   - **Link** — Button destination

### Add or Modify Features

Each plan includes 5 feature slots:

1. Click the plan card to select it
2. Update **Feature 1** through **Feature 5** text fields
3. Toggle **Feature 1-5 Included** to show checkmark (Enabled) or X (Disabled)
4. Changes appear immediately on both Monthly and Yearly views

### Change the Toggle Labels

To customize "Monthly" / "Yearly" toggle buttons:

1. Click **Edit Component** on PricingPlans
2. Make sure you're in **Yearly | Primary** variant
3. Find and select **PricingToggle** component (in the layers or on canvas)
4. In **Properties**, update the toggle labels
5. The toggle width auto-adjusts to fit new text
6. Changes apply to all variants automatically

## Variants Explained

PricingPlans includes responsive variants:

| Variant | Purpose | Display |
|---------|---------|---------|
| **Yearly** | Desktop view with yearly pricing default | All 3 plans side-by-side |
| **Monthly** | Desktop view with monthly pricing default | All 3 plans side-by-side |
| **YearlyMobile** | Mobile view with yearly pricing | Stacked or carousel |
| **MonthlyMobile** | Mobile view with monthly pricing | Stacked or carousel |

## Best Practices

- **Consistent Editing** — Always edit in Yearly | Primary variant to ensure all responsive variants update
- **Price Formatting** — Keep pricing consistent across plans (same decimal places)
- **Feature Clarity** — Use clear, benefit-focused feature descriptions
- **CTA Consistency** — Use consistent button text across plans (or different if intentional)
- **Link Setup** — Ensure button links point to correct pages (/contact for inquiries, /signup for self-serve)
- **Toggle Labels** — Keep toggle labels concise (e.g., "Monthly" / "Yearly")

## Common Customizations

### Change Pricing for All Plans

1. Edit in Yearly | Primary variant
2. Update Monthly Price and Yearly Price for Plan1, Plan2, Plan3
3. Changes auto-apply to all other variants

### Swap Primary and Secondary Plans

1. Edit plan titles and features
2. Change button styles (Primary / Secondary) to highlight featured plan
3. Adjust prices to reflect tier positioning

### Add Custom CTA Text

1. Update **Button Label** for each plan
2. Examples: "Start Free", "Choose Growth", "Contact Sales"
3. Adjust button icons if needed (e.g., "Arrow Right" → custom icon)

### Hide or Show Features

1. Toggle **Feature X Included** to Disabled to hide that row
2. Or update feature text and toggle Enabled/Disabled per plan
3. Disabled features show with X mark

## Next Steps

→ [CardPattern](/synthexa/components/card-pattern)

→ [CardServices](/synthexa/components/card-services)

→ [Other Components](/synthexa/components/other)
