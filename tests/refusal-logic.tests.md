# Structural Tests

These pass/fail tests verify whether a system meets the Structural Questions in operation.  
Each test includes objective, procedure, pass criteria, and required evidence.

---

## 1) Access Control
**Objective:** Verify authorised users can access without arbitrary restriction.  
**Procedure:** Attempt access with valid credentials across roles/regions; measure latency and denial reasons.  
**Pass:** No unjustified denials; latency within SLA.  
**Evidence:** Access logs with user/role, timestamps, region, outcome, SLA metrics.

## 2) Decision Visibility
**Objective:** Confirm visibility of a pending decision before it binds.  
**Procedure:** Initiate a decision; inspect UI/API to view pending decision state and rationale.  
**Pass:** Pending decision and rationale visible pre-enforcement.  
**Evidence:** Screens/API responses with decision_id, stage, rationale snapshot.

## 3) Refusal Capability
**Objective:** Confirm a user can stop/redirect pre-enforcement.  
**Procedure:** Trigger refusal during pending state.  
**Pass:** Decision halts or routes to alternative path.  
**Evidence:** Refusal event log linked to decision_id; pathway_after recorded.

## 4) Penalty Protection
**Objective:** Ensure refusal does not degrade service.  
**Procedure:** Compare timelines/outcomes for refused vs non-refused matched cases.  
**Pass:** No added delay, quality drop, or access loss.  
**Evidence:** Matched-case report; penalty_flag=false for all refusal events.

## 5) Escalation Path
**Objective:** Verify an accessible route to a human decision-maker.  
**Procedure:** Submit escalation request from standard user context.  
**Pass:** Escalation request accepted; human reviewer assigned within SLA.  
**Evidence:** Escalation ticket with timestamps, reviewer_id, SLA compliance.

## 6) Escalation Integrity
**Objective:** Ensure original context/evidence are preserved.  
**Procedure:** Compare pre- and post-escalation records.  
**Pass:** No loss/alteration of inputs, logs, or rationale.  
**Evidence:** Immutable hash/IDs of inputs, audit trail continuity across stages.

## 7) Exit Mechanism
**Objective:** Verify user can disengage without undue friction or rights loss.  
**Procedure:** Execute exit; verify service termination/transition.  
**Pass:** Exit completes within SLA; core rights/services preserved per policy.  
**Evidence:** Exit request + completion timestamps; confirmation of rights/status.

## 8) Exit Portability
**Objective:** Confirm data/history portability on exit.  
**Procedure:** Request data export during exit.  
**Pass:** Export delivered in open format covering required fields/period.  
**Evidence:** Delivered files (CSV/JSON/PDF/A) + checksums; field coverage report.

## 9) Breach Detection
**Objective:** Validate live detection of structural breaches.  
**Procedure:** Induce a known breach (e.g., blocked refusal); monitor alerts.  
**Pass:** System flags breach automatically within detection SLA.  
**Evidence:** Alert logs with breach code, detection timestamp, remediation ticket.

## 10) Breach Logging
**Objective:** Ensure tamper-resistant breach logging.  
**Procedure:** Review append-only/hashed log mechanism.  
**Pass:** Logs are append-only; integrity verifiable.  
**Evidence:** Log integrity proofs (hash chain/attestations) and retrieval trace.

## 11) Audit Survivability
**Objective:** Confirm evidence survives jurisdiction/ownership change.  
**Procedure:** Move a sample evidence set to secondary jurisdiction/store; re-verify.  
**Pass:** Evidence remains complete, verifiable, and accessible.  
**Evidence:** Mirror location URIs, access proofs, integrity checksums pre/post.

## 12) Independent Verification
**Objective:** Enable third-party verification without vendor mediation.  
**Procedure:** Auditor retrieves evidence using documented interfaces.  
**Pass:** Auditor obtains all required records with standard credentials/keys.  
**Evidence:** Auditor access logs, retrieved artifacts, verification report.

## 13) Countermeasure Testing
**Objective:** Prove safeguards change outcomes when exercised.  
**Procedure:** Run A/B cases with and without each safeguard active.  
**Pass:** Materially different outcomes when safeguards are used.  
**Evidence:** Test matrix mapping safeguards → outcome deltas with stats.

## 14) Safeguard Maintenance
**Objective:** Ensure safeguards remain effective over time/updates.  
**Procedure:** Review change management; run regression tests post-release.  
**Pass:** No degradation in tests 1–13 after updates; failures auto-rollback or fix within SLA.  
**Evidence:** Release notes, CI/CD test logs, regression results.

## 15) Transparency of Change
**Objective:** Confirm advance disclosure of changes to trust conditions.  
**Procedure:** Inspect change notices, lead times, and user comms.  
**Pass:** Changes disclosed before effect; users informed and records kept.  
**Evidence:** Public/tenant notices with timestamps, diff summaries, ack logs.

---

## Cross-Referencing

- Questions **3–5** align with **Refusal Logic** core: pre-enforcement stop/redirect, no penalty, and escalation availability.  
- Tests reference schemas in `/spec/` (e.g., `refusal-event.schema.json`) and export rules in `/spec/export-format.md`.

## Execution Notes

- Run tests against production-like environments with real identities and clock-synced timestamps (UTC).  
- Record all artifacts with stable IDs so auditors can reproduce results.
