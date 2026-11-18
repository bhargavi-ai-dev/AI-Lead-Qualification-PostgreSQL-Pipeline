# AI Lead Qualification & PostgreSQL Pipeline (n8n + Supabase)

An automated end-to-end lead processing pipeline built using **n8n**, **JavaScript Code Node**, **Groq LLM**, and **Supabase (PostgreSQL)**.

## Architecture & Workflow
1. **Webhook Ingestion:** Captures incoming lead submissions via a real-time HTTP Webhook.
2. **Custom Code Transformation:** Executes custom JavaScript logic to parse email domains and classify leads as `Corporate` or `Personal`.
3. **AI Priority Scoring:** Uses an LLM chain to analyze inquiry intent and assign a `High Priority` or `Low Priority` tag.
4. **PostgreSQL Persistence:** Inserts the structured, enriched lead record directly into a Supabase PostgreSQL table.
