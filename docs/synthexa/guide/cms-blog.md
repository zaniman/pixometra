# Blog Collection

The Blog collection powers your `/blog` page and blog post listing.

## Fields

| Field | Type | Notes |
|-------|------|-------|
| **Featured** | Boolean | Appears in blog homepage featured section |
| **Title** | String | Article headline |
| **Summary** | String | Short preview on the listing page |
| **Author** | Reference → Blog Authors | Select from Blog Authors collection |
| **Blog Category** | Reference → Blog Categories | Select from Blog Categories collection |
| **Date** | Date | Shown on listing and article page |
| **Main Image** | Image | Thumbnail and OG image |
| **Content** | Rich Text | Full article body — supports headings, links, formatting |
| **Read Time** | String | e.g. "5 min read" |
| **Slug** | String | URL path — auto-generated from title |


## Setup Order

:::warning
Create **Blog Authors** and **Blog Categories** BEFORE creating Blog posts.
:::

1. **Blog Authors** — Create author profiles first
2. **Blog Categories** — Create content categories
3. **Blog** — Now create blog posts (they reference Authors & Categories)

## Example Blog Post

**Title:** "How AI Automation Saved Our Client 200 Hours/Month"

**Slug:** `ai-automation-200-hours` (auto-generated)

**Summary:** "Discover how we implemented AI workflows that cut manual work in half."

**Author:** Select from Blog Authors

**Category:** Select from Blog Categories

**Content:** Full article text with markdown formatting

**Published Date:** April 16, 2024

**Read Time:** "8 min read"

**Featured:** Toggle on to show on blog homepage

## Auto-Generated Pages

Once saved, a new page is created at `/blog/:slug` with:
- Full article content
- Author info
- Category
- Publish date
- Related articles (if set up)
