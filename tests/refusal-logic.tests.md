# Structural Tests

These pass/fail tests verify whether a system meets the Structural Questions in operation.  
Each test includes objective, procedure, pass criteria, and required evidence.

---

# Category 1 - User Agency Removal
## 1.	Refusal Prevention
Standard:  A system must allow users to say no without penalty.  Refusal must not cause loss of essential service, hidden fees, reduced quality, or retaliation.  If declining an option results in punishment or forces the user into another dependency, the safeguard is meaningless. Refusal must remain a safe, equal, and respected choice.
Question:  Can any user stop or redirect a decision at any point without penalty or loss of service? 
How to test:
•	Click “no” or decline an option in the system.
•	Check if the service continues normally (no penalties, extra charges, or downgrades).
•	If the service is cut, reduced, or costs more, mark fail.

## 2.	Escalation Suppression
Standard:  A system must provide real routes of appeal when decisions are contested.  An appeal that loops back to the same authority, or to staff without power to reverse outcomes, is not valid.  If escalation is denied, delayed until meaningless, or designed to exhaust the user into giving up, the system breaches trust. Escalation must be independent, timely, and empowered to correct harm.
Question:  Can any user trigger escalation to a human with authority, with that escalation logged to resolution?
How to test: 
•	Complain about a decision and ask to escalate it.
•	Observe if the case reaches a human with authority to change the outcome.
•	If it loops back, stalls, or ends without authority, mark fail.
Note: Escalation must be logged and resolved (not just acknowledged).
 
## 3. Exit Obstruction
Standard:  A system must allow users to leave without excessive cost, harm, or loss.  Locking people in through data deletion, high switching fees, or withdrawal of unrelated services is not a free exit.  If leaving exposes the user to new risks, the option is not real.  Exit must be safe, practical, and non-punitive.
Question:  Can any user leave the AI pathway and continue receiving the same core service without delay, cost, or requalification?
How to test: 
•	Try to leave the AI process while keeping the core service (e.g. opt out of AI recommendations but still use the platform).
•	Observe if this exit is allowed without new costs, delays, or requalification.
•	If exit blocks or harms service access, mark fail.

## 4. Access Gating
Standard:  A system must ensure equal access to safeguards and protections.  Making appeals, human review, or essential support available only to premium customers, certain languages, or those with specific IDs creates unfair barriers.  Protection must not depend on wealth, geography, or privilege.
Question:  Are safeguards and human alternatives available equally to all users, regardless of geography, payment tier, or identity verification?
How to test: 
•	Attempt to use safeguards (appeal, human review) from a low-tier account, in another language, or without ID.
•	Observe whether protections are equal to those offered to premium or verified users.
•	If safeguards differ by tier, language or ID, mark fail. 

Category 2 - Visibility & Traceability Gaps


## 5. Traceability Void
Standard:  A system must keep records of how and why decisions are made.  If no audit trail exists, or the process is too complex to reconstruct, accountability disappears.  Users must be able to see what influenced a decision, regulators must be able to verify it, and operators must be answerable for it.  Without traceability, trust collapses.
Question:  Can the exact model, version, and decision chain be identified for every output?
How to test:
•	 Ask: ‘Show me the exact model, data, and steps used for decision X” - request both the decision logic and the specific data used.
•	Observe whether a full, step-by-step record is provided.
•	If no clear decision chain is shown, mark fail.

## 6. Memory Erasure
Standard:  A system must retain evidence of its past actions long enough to expose repeated harm.  If records are deleted, fragmented, or hidden, patterns of abuse appear as isolated mistakes.  Users and regulators must be able to see history, not just the present moment.  Without memory, harm repeats without proof.
Question:  Are harm events logged and retained long enough to detect and act on repeat or systemic failure?
How to test: 
•	Request logs of past harm incidents over the last 3 months.
•	Observe whether a continuous history of complaints and outcomes is shown with proof (e.g., confirmation with timestamp).
•	If logs are missing, fragmented, or reset, mark fail.

## 7. Evidence Nullification
Standard:  A system must provide evidence that can stand up to scrutiny.  Data that is incomplete, editable, unverifiable, or locked in inaccessible formats cannot be used to prove harm.  If records exist but fail as proof, they serve the operator, not the user.  Evidence must be durable, verifiable, and usable in disputes.
Question:  Can harm records be exported and presented in a regulator- or court-admissible format?
How to test: 
•	Ask for harm records in a format usable by regulators (e.g. PDF with timestamps).
•	Observe if the file is complete, uneditable and readable.
•	If the file is incomplete or cannot be used as proof, mark fail.

## 8. Time Suppression
Standard:  A safeguard delayed is a safeguard denied.  If complaint systems, appeals, or reviews take longer than the harm itself, rights exist only on paper.  Delay must not be used as a tactic to let deadlines expire, evidence vanish or harm become irreversible.  Safeguards must act fast enough to prevent lasting damage.
Question:  Are refusal, escalation, and review completed within enforceable deadlines with auditable timestamps?
How to test: 
•	File a complaint and record the time.
•	Observe whether the case is resolved within enforceable deadlines (e.g. 30 days).  Interim responses must include a plan with milestones.
•	If the deadline is missed or delayed, mark fail.

 # Category 3 - Simulation & Misrepresentation

## 9. Simulation Logic
Standard:  A system must not pretend protections exist when they do not.  Policies, dashboards, or safeguards that look good in design but do nothing in practice mislead users into false trust.  If a right exists only on paper or in a menu, but never changes outcomes, it is a breach.  Safeguards must be real, functional, and enforceable.
Question:  Do all stated safeguards operate exactly as described when tested in live conditions?
How to test: 
•	Use every safeguard (appeal, opt-out, review) and verify each changes outcomes.
•	Observe whether the safeguard actually changes the outcome.
•	If nothing changes beyond a confirmation screen, mark fail.

## 10. Simulated Consent
Standard:  Consent must be genuine.  If users are told they have a choice but refusal means losing essential services, being downgraded, or facing hidden costs, then the “choice” is a lie. Clicking “accept” under duress is not consent.  Real consent means saying yes or no without fear of punishment.
Question:  Can a user refuse consent and still access an equal-value, non-AI pathway?  
How to test: 
•	Refuse consent when prompted (e.g. “Do not track”).
•	Observe if you can still use the service fully and equally.
•	If refusal downgrades or blocks access, mark fail.

## 11. Metric Gaming
Standard:  Metrics must measure real outcomes, not theatre.  If an organisation tracks numbers that hide harm (like “tickets closed” instead of “problems solved”), the data is meaningless.  When numbers are chosen to make systems look good while ignoring harm, they block accountability.  Metrics must reveal reality, not disguise it.
Question:  Do performance measures track verified harm resolution rather than proxy indicators?
How to test: 
•	Ask for the company’s performance metrics (e.g. “tickets closed”) and raw complaint logs.
•	Observe whether these metrics reflect real harm resolution (e.g. “problems solved”).
•	If metrics disguise or hide harm, mark fail.

 # Category 4 - Accountability & Jurisdiction Evasion
 ## 12. Cross-Accountability Gap
Standard:  Accountability must follow harm across the chain.  If every actor points elsewhere: the platform blames the vendor, the vendor blames the regulator, the regulator blames the law, harm becomes visible but no one takes responsibility.  A system is in breach if it leaves users caught in this loop.  Responsibility must remain clear, shared, and enforceable.
Question:  Can every actor in the chain be named and held contractually responsible for repairing harm?
How to test: 
•	Ask until you get a named person/role (not a department or ‘team’).
•	Observe whether a clear, named actor takes responsibility.
•	If responsibility shifts between parties or is unclear, mark fail.

## 13. Jurisdiction Displacement
Standard:  A system must not move decisions or data into spaces where oversight cannot reach.  Shifting storage overseas or routing appeals into jurisdictions without real enforcement, strips rights of their power. Protection on paper must equal protection in practice, wherever the system operates.
Question:  Can local authorities compel the system to halt, change, or reverse harmful actions?
How to test: 
•	Issue a local regulator order (e.g. “Stop action Y”).
•	Observe whether the operator complies under your authority.
•	If they claim it lies outside your jurisdiction or control, mark fail.

## 14. Enforcement Bypass
Standard:  A system must not be designed to step around the spirit of rules while obeying the letter.  If protections exist but are neutralised by loopholes, technicalities, or proxy arrangements, enforcement has been bypassed.  True compliance means obeying both the rules and their intent.
Question:  Are there no architectural or contractual exemptions that remove applicable legal duties?
How to test:
•	Review contracts or system design for compliance terms.
•	Observe whether safeguards apply without loopholes or exemptions.
•	If duties are bypassed by design or contract, mark fail.

## 15. Harm Scope Narrowing
Standard:  A system must recognise the full range of harm it causes.  If it defines harm so narrowly that financial loss counts but emotional damage, dignity, or exclusion do not, users are denied real remedy.  Harm must be defined as people experience it, not as systems prefer to record it.
Question:  Does the harm definition include emotional, reputational, and cumulative damage with a route to redress?
How to test:
•	Ask, “Does your harm definition include emotional and reputational damage?”
•	Observe whether definitions include financial, emotional, reputational, and cumulative harm.
•	If harm is defined only as financial loss, mark fail.
 

## Execution Notes

- Run tests against production-like environments with real identities and clock-synced timestamps (UTC).  
- Record all artifacts with stable IDs so auditors can reproduce results.
