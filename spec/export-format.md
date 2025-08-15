# Refusal Logic Export Format

This format is designed for regulatory and cross-jurisdictional review. It is intentionally minimal and structured for both machine parsing and human inspection.

## File Formats
- **Primary:** JSON Lines (`.jsonl`)
- **Alternate:** CSV (`.csv`) with UTF-8 encoding

## Required Fields
| Field | Type | Description |
|-------|------|-------------|
| event_id | string | Unique ID for the refusal event |
| timestamp | datetime (UTC) | When refusal occurred |
| decision_id | string | Links to the original decision |
| triggered_by | string | ID of triggering user/process |
| jurisdiction | string | Country/region code |
| pathway_before | string | Pathway before refusal |
| pathway_after | string | Pathway after refusal |
| penalty_flag | boolean | Should be false in compliant systems |
| reviewer_id | string (optional) | Oversight reviewer ID |
| outcome | string | Result after refusal |

## JSON Lines Example
```json
{"event_id":"abc123","timestamp":"2025-08-18T10:00:00Z","decision_id":"dec789","triggered_by":"user456","jurisdiction":"GB","pathway_before":"AI_auto_approval","pathway_after":"manual_review","penalty_flag":false,"reviewer_id":"auditor99","outcome":"approved"}
