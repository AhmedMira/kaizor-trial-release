# KAIZOR Platform — Technical Overview (No Source)

This document is a **technical overview** intended for engineering‑heavy organizations evaluating KAIZOR.
It contains **no source code** and focuses on real operational problems and how KAIZOR addresses them.

## 1) Reality-driven problem framing

### Asset reality
- Asset inventories are incomplete and drift over time.
- Different teams track different “truths” (CMDB vs cloud vs spreadsheets).
- Exposure changes quickly (temporary hosts, short‑lived services, environment sprawl).

### Finding reality
- Scan outputs are noisy and often duplicated across runs.
- Severity labels alone are not sufficient for remediation planning.
- Ownership is unclear: a finding might belong to infra, app, platform, or a vendor.

### Workflow reality
- Findings are lost in tickets, email, and spreadsheets.
- Status definitions vary between teams (what “fixed” means, when “accepted risk” is valid).
- Reporting is manual and non-repeatable.

## 2) What KAIZOR provides (conceptual)

### A unified findings workflow
KAIZOR treats findings as first-class entities with a clear lifecycle, enabling:
- consistent triage
- reproducible status changes
- clear communication across security and engineering

### A practical asset model
KAIZOR tracks assets as real-world identifiers (e.g., hostnames, IPs, domains, services) to support:
- filtering and searching by asset context
- connecting scan outputs to a living inventory

### A repeatable reporting surface
KAIZOR provides a “latest report” view intended to reduce manual reporting effort and allow a consistent picture of current risk.

## 3) Ingestion and supported inputs (Trial)

The trial is built to validate the real operational loop:
1. add assets
2. ingest scan outputs
3. review findings
4. update status
5. review report

Supported trial inputs include common formats such as:
- Nessus exports
- Nmap XML output

## 4) Operating model (local trial)

### Local-only runtime
- Runs on loopback (local machine only)
- Designed to be easy to start and evaluate without network reconfiguration

### Activation model
- Trial is activated using a shared trial key
- Duration is **48 hours**, starting at activation time

## 5) Security and privacy posture (trial)

The trial is designed to be evaluated without requiring customers to expose infrastructure publicly.
Typical evaluation expectation:
- run locally
- import sanitized scan outputs (if needed)
- validate workflow and reporting value

## 6) What to evaluate in a technical review

### Workflow fit
- Can your team map your real statuses to the available states?
- Does it reduce the time spent in triage and reporting?

### Noise reduction and usability
- Can you quickly locate high-impact findings?
- Can you find findings by asset context and search terms?

### Reporting credibility
- Does the report capture the story you need for leadership?
- Is it consistent across repeated runs?

## 7) Trial limitations (expected)

The trial is intentionally focused on core workflow validation:
- It is not a complete enterprise rollout (no large-scale integrations are implied here).
- It is optimized for evaluation speed, not organization-wide deployment.

## 8) Support

If you want a technical walkthrough for your environment (asset model, scan formats, workflow mapping), share:
- sample (sanitized) scan files
- your target workflow states
- what “success” means for your team during the 48h window

