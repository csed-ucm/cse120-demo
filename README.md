## CSE Capstone (Agile Redesign) Concise Summary 

This update replaces Lab 4 (4.1–4.4) and Lab 5 with five agile iterations and keeps Labs 1–3 as planning. Meeting minutes are replaced by GitHub artifacts (issues/PRs/reviews/tags/releases) plus a lightweight Weekly Status Report issue. Labs are protected collaboration time for planning, building, testing, documentation, release, and a short demo; the TA verifies progress via artifacts and the in-lab demo.

### Structure at a glance
- Planning Labs (3): Planning A, B, C (Weeks 1–6 windows; due Weeks 3, 5, 6)
- Implementation Iterations (5): Iterations 1–5 (Weeks 6–17 windows; key due points aligned below)
- Weekly cadence: plan → build via PRs → test → doc → tag/release → demo → status report

### Planning Labs (keep Labs 1–3)
- Planning A (Lab 1; Due Week 3): Teams, repo/CI, charter, Working Agreement, DoD/DoR, backlog seed, PR/issue templates.
- Planning B (Lab 2; Due Week 5): Discovery, stakeholder mapping, prioritized backlog (10–20 items), ADRs started, risk register.
- Planning C (Lab 3; Due Week 6): MVP and 5-iteration roadmap, test strategy, acceptance criteria style.

Artifacts (each planning lab): reviewed PRs updating README/CONTRIBUTING/templates/ADRs/backlog; team Weekly Status Report issue linking artifacts and readiness.

### Implementation Iterations (replace 4.1–4.4 and 5)
- Iteration 1 (Weeks 6–8; due Week 8, Design Reviews): v0.1 thin vertical slice; demo at Design Reviews.
- Iteration 2 (Weeks 9–11; due Week 11; Midterm assigned ~Week 9; Spring Break Week 10): v0.2 core+APIs+data.
- Iteration 3 (Weeks 12–13; due Week 13): v0.3 UX + observability/operability; unhappy paths.
- Iteration 4 (Weeks 14–15; due Week 15): v0.4 security + performance; P0 fixes.
- Iteration 5 (Weeks 16–17; RC Week 16; final Week 17 for I2G): v1.0-rc → v1.0; docs/poster/handoff.

Required artifacts (each iteration):
- Tagged release and notes; 3–5 merged PRs per student across the iteration
- Tests added/updated; CI green; coverage/lint/scan gates pass
- Updated docs (README/Guides/ADRs/Runbook) + CHANGELOG
- 3–5 min demo in lab + team Weekly Status Report issue linking all artifacts

Due cadence: demo in lab by Friday; release tag + Status Report Sunday 11:59pm (adjust for midterm/holidays as directed).

### Five-person rotation (per iteration)
Roles per iteration (rotate so each student serves in each role once):
- Iteration Lead: runs planning, manages board, ensures DoD, posts Status Report.
- Backend Lead: domain/APIs/data contracts and migrations.
- Frontend/UX Lead: flows, accessibility, acceptance tests.
- QA/Testing Lead: testing strategy, coverage gate, flake triage, release verification.
- DevOps/Release Lead: CI/CD, quality gates, preview envs, tagging/releases, telemetry.

Example rotation across Iterations 1–5
- A: Lead → Backend → Frontend → QA → DevOps
- B: Backend → Frontend → QA → DevOps → Lead
- C: Frontend → QA → DevOps → Lead → Backend
- D: QA → DevOps → Lead → Backend → Frontend
- E: DevOps → Lead → Backend → Frontend → QA

Presentation/review rotation: two presenters per iteration; reviewers assigned across different focus roles.

### Policies (replace meeting minutes)
- Weekly Status Report (team-level GitHub issue) includes: sprint goal/scope; done items with PR/issue links; release tag; CI status; tests/coverage; risks/blocks; next goal; individual contributions (PRs/reviews/hours).
- PR rules: linked issue and acceptance criteria; tests+docs; CI green; ≥1 reviewer; small/focused PRs; co-authored-by trailers for pair/mob.
- Contribution tracking: evaluated via authored PRs, meaningful reviews, commits tied to issues, and demo attribution.

### Alignment to your date grid
- Week 8: Design Reviews → Iteration 1 demo, v0.1 tag
- Week 9 assigned / Week 10 due: Midterm overlaps Iteration 2 (lighter sprint due to Spring Break)
- Week 16: Project Initial Draft → aligns to v1.0-rc
- Week 17: Innovate 2 Grow → final v1.0 release, poster, handoff

### Instructor/TA cadence
- Before lab: scan PRs/releases/CI and Status Report issue
- In lab: demos, spot checks, risk/quality Q&A
- After lab: comment on the Status Report with approval or change requests

Notes: Labs are protected team time; lectures remain lighter-touch and supportive of the above focuses. Adjust cutoff day to match your section’s lab day if needed.
