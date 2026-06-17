# Kaizor Platform — Visual Diagrams

These diagrams are documentation-only and contain **no source code**.

## 1) Platform map (capability tracks)

```mermaid
flowchart TB
  A[Real-world inputs<br/>docs • tickets • scans • chats • screenshots] --> B[Understanding & Synthesis]
  B --> C[Decision Support]
  C --> D[Governed Execution]
  D --> E[Outcomes & Reporting]

  B --> K[Knowledge capture]
  E --> K
  K --> B

  subgraph Tracks[Capability Tracks]
    T1[Knowledge & Synthesis]
    T2[Workflow Orchestration]
    T3[Controlled Automation]
    T4[Multi-modal Interaction]
  end
```

## 2) From problem to outcome (human-in-the-loop)

```mermaid
sequenceDiagram
  participant User
  participant Kaizor
  participant Systems as Tools/Systems

  User->>Kaizor: Describe the situation / goal
  Kaizor->>Kaizor: Summarize + extract key context
  Kaizor->>User: Proposed plan + choices
  User->>Kaizor: Approve / adjust
  Kaizor->>Systems: Execute safe actions (governed)
  Systems-->>Kaizor: Results
  Kaizor->>User: Final summary + next steps
```

## 3) Governance model (trust boundaries)

```mermaid
flowchart LR
  L[Low-risk steps] --> A1[Auto-execute]
  H[High-impact steps] --> A2[Require confirmation]
  A2 --> Log[Audit trail]
  A1 --> Log
  Log --> Review[Reviewable history]
```

## 4) Where the Trial fits (one capability track)

```mermaid
flowchart TB
  P[Kaizor Platform] --> C1[CyberSec Capability Track]
  P --> O1[Other capability tracks]

  C1 --> T[This Trial]
  T --> A[Assets]
  T --> U[Scan uploads]
  T --> F[Findings workflow]
  T --> R[Latest report]
```

