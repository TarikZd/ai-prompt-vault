# Template Audit & Friction Points — AI Prompt Vault

## 1. Logo Hosting Issue (Notion API)
- **Problem:** The Notion API `icon` property does not support direct local file uploads; it only accepts external URLs or native emoji icons.
- **Resolution:** The `moorish_dev_logo.png` has been distributed to `assets/`. User must drag-and-drop the logo as the page icon manually in the Notion UI after template generation, or provide a public CDN URL.

## 2. Formula 2.0 Manual Conversion Required
- **Problem:** The Notion API does not support creating `Formula` property types directly via API calls in all contexts. The formula property may be created as a Rich Text placeholder during automated generation.
- **Resolution:** User must manually open the database property settings, change the type to `Formula`, and paste the formula snippet documented in `docs/Database_Schema.md`.

## 3. Linked View Limitation
- **Problem:** The Notion API can create database views, but certain advanced view settings (filters, sorts, groupings) must be configured manually in the Notion UI.
- **Resolution:** After the automated build creates the `[DB] Backend` sub-page and the Linked View, the user must open the Linked View and manually set filters/sorts as described in `setup_guide/Setup_Guide.md`.

## 4. Button Block API Limitation
- **Problem:** Notion's native Button blocks (automations) cannot be created or configured via the public Notion API.
- **Resolution:** The `TASKS.md` build task includes a `[BUTTON]` step, but this must be executed manually by the user inside the Notion UI following the instructions in `setup_guide/Setup_Guide.md`. The task will be marked `[/]` until this manual step is confirmed.

## 5. Synced Block Cross-Page Linking
- **Problem:** Synced Blocks must be created on one page and then "synced" to other pages. The Notion API supports creating synced block copies, but the source synced block must exist first.
- **Resolution:** The Navigation Synced Block will be created on the main dashboard page first. All sub-pages will reference it. This is a known limitation and will be noted in the Setup Guide.

## 6. Long Text Formatting Limits
- **Problem:** Notion page body text is separate from database properties. Storing long prompts in text properties cuts off spacing.
- **Resolution:** Instruct users to write prompt bodies directly on the page body itself. Database properties should only store variables, tags, and titles.
