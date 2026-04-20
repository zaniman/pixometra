# CardFAQ & FAQAccordion

An expandable accordion component that displays frequently asked questions with numbered items and detailed answers. Used on the homepage FAQ section to address common customer questions.

![FAQAccordion](/images/guide/synthexa-94@2x.png)

## Overview

**FAQAccordion** is the main container component that includes:
- Multiple FAQ items organized in an accordion
- Collapsible/expandable question-answer pairs
- Numbered questions (01, 02, 03, etc.)
- Responsive variants for different question states

**CardFAQ** is an individual question-answer item with:
- Question number
- Question title
- Detailed answer text
- Expand/collapse interaction

## How to Edit

### Edit with Edit Component

To customize FAQ items:

1. **Select FAQAccordion** on the canvas OR in the **Layers** panel
2. Click **Edit Component** button in Properties
3. You'll see variants for each question state:
   - **0 | Primary** — The main/primary state (edit here)
   - Additional variants for other expanded question states

![Edit with Edit Component](/images/guide/synthexa-95@2x.png)

:::warning
**Always make FAQ edits in the 0 | Primary variant.** Changes automatically apply to all other variants.
:::

### Edit Individual Questions

To edit a specific question and answer:

1. Find and click on the specific question (CardFAQ component) in layers or canvas
2. In **Properties**, update:
   - **Number** — Question number (e.g., "01", "02")
   - **Title** — The question text
   - **Description** — The full answer text

![Edit Individual Questions](/images/guide/synthexa-96@2x.png)

## Add a new question

**Step 1: Add the question to 0 | Primary variant**
1. Click **Edit Component** on FAQAccordion
2. In the **0 | Primary** variant, find the CardFAQ list
3. Duplicate an existing CardFAQ (e.g., duplicate question 07)
4. Update the new question:
   - **Number** — New question number (e.g., "08")
   - **Title** — Question text
   - **Description** — Answer text

**Step 2: Create a new variant for the expanded question**
1. Still in **Edit Component** mode
2. Select the last variant button (e.g., the "7" button)
3. In variant 7, make sure the new question 08 has **Variant** set to **Closed**
4. Click **+ Variant** button to create a new variant
5. Name the new variant with the question number (e.g., "8")

![Create a new variant for the expanded question](/images/guide/synthexa-97@2x.png)

**Step 3: Configure the new variant**
1. Click on the newly created variant (e.g., "8")
2. For all other questions (01-07):
   - Select each CardFAQ
   - In **Properties**, set **Variant** to **Closed**
3. For the new question (CardFAQ with number 08):
   - Select it
   - In **Properties**, set **Variant** to **Open** (to show expanded state)
   - This is the only question shown open in this variant

![Configure the new variant](/images/guide/synthexa-98@2x.png)

**Step 4: Set up Interactions**
1. Go back to **0 | Primary** variant
2. Select the new question component (CardFAQ with number 08)
3. In **Properties**, go to **Interactions** section

![Interactions](/images/guide/synthexa-99@2x.png)

4. Click **7** to change the interaction
5. Link the interaction to the new variant (e.g., variant "8")

![Interactions](/images/guide/synthexa-100@2x.png)

## Reduce the number of questions

1. Click **Edit Component** on FAQAccordion
2. In the **0 | Primary** variant, select the question to delete (e.g., question 07)
3. Press **Delete** key or right-click and select **Delete**
4. Then delete the corresponding variant:
   - Click on the variant number button (e.g., the blue "7" button)
   - Press **Delete** key to remove that variant
5. Update remaining question numbers if needed

