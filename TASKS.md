# 📋 Free Templates: Active Tasks — AI Prompt Vault

This document tracks all development tasks for this template, strictly adhering to the `AGENTS.md` protocol. When a task is fully verified, the agent must append it to `TASKS_ARCHIVE.md` with required Handoff Notes.

- `[ ]` uncompleted tasks
- `[/]` in progress tasks
- `[x]` completed tasks

---

## 🏃 Current Sprint

### Local Filesystem Initialization
- [x] **T0: [DESIGN] Create Local Directory Structure and Apply Logo** — *(completed 2026-06-19 by Antigravity)*
  - **Changed:** Created subdirectories (`assets/`, `docs/`, `marketing/`, `notion_screenshots/`, `setup_guide/`) and copied `moorish_dev_logo.png` into `assets/`.
  - **Gotchas/Next Steps:** Proceed to REFACTOR task T0.01 to build the Notion template.

### 🛠️ Refactoring & Build
- [ ] **[REFACTOR] | T0.01 | ⚡CRITICAL — Build AI Prompt Vault Notion Template**
  - **Impact:** `/AI Prompt Vault/notion_screenshots/`, `/AI Prompt Vault/docs/`
  - **Details:** Build the full Notion template following the structural pattern from `AGENTS.md`:
    1. **[ARCHITECTURE]** Create `[DB] Backend` sub-page. Move the master databases inside. Create a Linked View on the main dashboard.
    2. **[FORMULA]** Add Formula 2.0 `Variables Tracker` which parses and counts prompt variables `[like_this]` dynamically, and `Model Tag` builder.
    3. **[NAVIGATION]** Create a Synced Block at the top for the Navigation Menu.
    4. **[FOOTER]** Create a Synced Block at the bottom (The Traffic Footer) with a link to the Notion Creator Profile and Moorish Dev brand mention.
    5. **[SEO]** Add a Toggle at the bottom titled `[Admin] SEO Metadata` with SEO Title, Meta Description, and 10 Keywords.
    6. **[BUTTON]** Add a Notion Button block labeled "➕ New Prompt" and "📝 Create Version" that creates new items.
    7. **[CALLOUT]** Add a Gray Background Callout titled "How to Use" with quick steps to setup.
  - **Affiliate Check:** N/A

### 📄 Documentation
- [ ] **[CONTENT] | D1.01 | 🔴 HIGH — Populate `docs/Database_Schema.md`**
  - **Impact:** `/AI Prompt Vault/docs/`
  - **Details:** Document all database properties, Formula 2.0 logic, and Vault architecture.

- [ ] **[CONTENT] | D1.02 | ⚠️ MEDIUM — Populate `marketing/Launch_Copy.md`**
  - **Impact:** `/AI Prompt Vault/marketing/`
  - **Details:** Write 3 Twitter hooks and 1 Product Hunt-style description targeting AI Prompt Vault keywords.

- [ ] **[CONTENT] | D1.03 | ⚠️ MEDIUM — Populate `setup_guide/Setup_Guide.md`**
  - **Impact:** `/AI Prompt Vault/setup_guide/`
  - **Details:** Write a step-by-step "Start Here" user guide.

### 🚀 Launch
- [ ] **[MARKETING] | L1.01 | 🟢 LOW — Publish to Notion Template Gallery**
  - **Impact:** External
  - **Details:** Submit the duplicated Notion template link to the Notion Template Gallery and relevant communities.

---

## Summary

| Phase | Tasks | Done | Remaining |
|-------|-------|------|-----------|
| Init & Structure | 1 | 1 | 0 |
| Build & Refactor | 1 | 0 | 1 |
| Documentation | 3 | 0 | 3 |
| Launch | 1 | 0 | 1 |
| **TOTAL** | **6** | **1** | **5** |

> **Priority Order**: T0.01 → D1.01 → D1.02 → D1.03 → L1.01
