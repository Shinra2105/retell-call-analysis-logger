**AI Voice Agent Analysis & CRM Logging Pipeline**
**Automates post-call analysis from Retell AI, logging transcripts, sentiment, and conversion data into Airtable and Kommo CRM.**

Description: This workflow acts as a backend listener for Retell AI voice agents. It receives call_analyzed webhooks and performs a detailed breakdown of the interaction.

Key Features:

Dynamic Logic: Uses a Switch node to filter calls based on duration (<15s vs >15s) and outcome (Appointment Confirmed/Denied).

Data Enrichment: Calculates call costs, duration, and extracts custom LLM variables (e.g., user sentiment, refusal reason).

Multi-Platform Sync:

Airtable: Creates comprehensive logs for analytics (Cost per call, Confirmation rates).

Kommo CRM: Updates lead status and adds notes based on the AI's conversation summary.
