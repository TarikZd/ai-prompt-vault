# 🗄️ Database Schema: AI Prompt Vault
---
## Primary Database: Prompts
| Property Name | Type | Purpose |
| --- | --- | --- |
| **Prompt Name** | `Title` | Short name/use-case. |
| **Category** | `Select` | `Writing`, `Coding`, `Data Extraction`, `SEO`, `Design`. |
| **Target Model** | `Multi-select` | `GPT-4o`, `Claude 3.5 Sonnet`, `Gemini Pro`. |
| **Prompt Text** | `Text` | The prompt template. |
| **Variables** | `Text` | Dynamic fields. |
