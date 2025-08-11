# CSE Capstone (Agile Redesign) — Concise Summary

- This update replaces Lab 4 (4.1–4.4) and Lab 5 with five agile iterations and keeps Labs 1–3 as planning.
- Meeting minutes are replaced by GitHub deliverables: issues, PRs, reviews, tags, releases, project boards
- Labs are protected collaboration time for planning, building, testing, documentation, release, and a short demo.
- The TA verifies progress via deliverables and the in-lab demo.

## Structure at a glance

- Planning Labs (3): Planning A, B, C (Weeks 1–6 windows; due Weeks 3, 5, 6)
- Implementation Iterations (5): Iterations 1–5 (Weeks 6–17 windows)

## Planning Labs (keep Labs 1–3)

### Planning A (Lab 1; Due Week 3)
- [ ] Repo, GitHub Project Board, 
- [ ] Working Agreement, 
- [ ] DoD/DoR (Definition of Done vs. Definition of Ready),
- [ ] backlog seed (initial items or features that are added to the product backlog)
- [ ] PR/issue templates

### Planning B (Lab 2; Due Week 5):
- [ ] Discovery (researching user needs, market analysis, and technical feasibility)
- [ ] Stakeholder mapping (identifying and analyzing stakeholders' interests and influence)
- [ ] Prioritized backlog with milestones (milestones must have a clear acceptance criteria and sub-tasks)
- [ ] ADRs started (Architecture Decision Records, software stack, monolith vs. microservices, platform choices, etc.)
- [ ] Risk register (identifying and assessing project risks like if a student drops the course, or students will only be able to visit test site at certain times)

### Planning C (Lab 3; Due Week 6):
- [ ] MVP and 5-iteration roadmap (defining the minimum viable product and planning the next five iterations)
- [ ] Test strategy (unit, integration, end-to-end)
- [ ] Acceptance criteria style (Given-When-Then format)

Deliverables (each planning lab): reviewed PRs updating README/CONTRIBUTING/templates/ADRs/backlog; team Weekly Status Report issue linking deliverables and readiness; GitHub Project Board updated.

## Implementation Iterations (replace 4.1–4.4 and 5)

### Weekly agenda:

1. **Plan**
2. **Research (Optional)**
3. **Build**
4. **Test**
5. **Create a PR**
6. **PR review**
7. **Documentation**
8. **PR pulled**
9. **Tag/Release (Graded)**
10. **Status report and deliverables**

### Iterations:

- Iteration 1 (Weeks 6–8; due Week 8, Design Reviews)
- Iteration 2 (Weeks 9–11; due Week 11; Midterm assigned ~Week 9; Spring Break Week 10)
- Iteration 3 (Weeks 12–13; due Week 13)
- Iteration 4 (Weeks 14–15; due Week 15)
- Iteration 5 (Weeks 16–17; RC Week 16; final Week 17 for I2G)

### Typical iteration goals:

- core components
- APIs framework
- data structures
- proof of concept experimentations and demos
- UX
- Security + performance; P0 fixes.
- Docs/poster/handoff.

### Required deliverables (each iteration):

- Tagged release and notes; 3–5 merged PRs per student across the iteration
- Tests added/updated; CI green; coverage/lint/scan gates pass
- Updated docs (README/Guides/ADRs/Runbook) + CHANGELOG
- 3–5 min demo in lab + team Weekly Status Report issue linking all deliverables

### Due dates
- Demo in lab or office hours by Friday;
- PRs merged by Sunday 11:59pm.
- One extra week for report (but only if PRs merged on time and released)
- Students are given **1 additional extension** for up to 1 week for PR merges or demos.

## Five-person rotation (per iteration)

Rotate roles so each student serves in each role at least once or as evenly as possible across the team. For instance, each member should try at least one rotation in each role over the course of the project.

### Typical Roles:
- Iteration Lead: runs planning, manages board, ensures DoD, posts Status Report.
- Backend Lead: domain/APIs/data contracts and migrations.
- Frontend/UX Lead: flows, accessibility, acceptance tests.
- QA/Testing Lead: testing strategy, coverage gate, flake triage, release verification.
- DevOps/Release Lead: CI/CD, quality gates, preview envs, tagging/releases, telemetry.

### Presentation/review rotation: 

Two or three presenters per iteration; reviewers assigned across different focus roles based on progress. This can allow students to better strategize their presentations based on the completion level of various features.

## Typical iteration

### Learning objectives (mapped to common capstone outcomes):
- Apply software engineering process to plan, implement, test, and evaluate a feature increment.
- Practice technical communication via PRs, reviews, and release notes.
- Demonstrate teamwork, role flexibility, and time management.
- Produce reproducible results with evidence (tests, CI logs, release tag).

### Inputs
- Definition of Ready stories with acceptance criteria and scope sized for one iteration.
- Updated backlog with priorities informed by prior feedback and risks.

### Activities (recommended)
- Planning (30–45 min in lab): confirm sprint goal, assign roles for the iteration, select stories, and clarify acceptance criteria.
- Development in small PRs: pair where helpful; link PRs to issues; request reviews early.
- Testing: add unit/integration tests; if relevant, add data fixtures or UI tests.
- Documentation: update README/Guides/ADRs; record notable decisions in ADRs.
- Release: tag with semantic version (e.g., v0.2.0), write brief notes (what/why/how verified).
- Demo: 3–5 minutes showing the increment, tests passing, and any metrics.

### Assessment (suggested rubric per iteration)
- Technical correctness and functionality — 40%
- Process and quality (PR hygiene, small changes, reviews, CI green) — 20%
- Testing depth and reliability (coverage appropriate to scope, edge cases) — 15%
- Documentation and communication (README/ADRs/release notes) — 15%
- Professionalism/teamwork (role fulfillment, responsiveness, equitable contribution) — 10%

### Time expectations
- ~6–8 hours/student/week (30–40 team-hours). Scope stories accordingly; defer stretch items.

### Examples of iteration goals by project type (undergraduate scope)
Web/API application
- Iteration 1: Auth-less vertical slice (one entity): create/list UI, simple API, in-memory/SQLite data, basic tests.
- Iteration 2: Persistence + auth-lite: migrations, CRUD APIs, error handling, contract tests, 2–3 UI flows.
- Iteration 3: UX polish + observability: form validation, a11y checks, structured logs, health checks.
- Iteration 4: Performance + security: naive cache, pagination, rate-limit, dependency scans, fix P0 bugs.
- Iteration 5: Release candidate: docs completeness, onboarding script, seed data, final polish.

Data/ML workflow
- Iteration 1: Data audit + baseline: small curated dataset, baseline model or heuristic, evaluation script, tests.
- Iteration 2: Feature pipeline + storage: versioned datasets, preprocessing, metrics logging.
- Iteration 3: Model improvement: one architecture or hyperparameter change with fair comparisons.
- Iteration 4: Robustness + error analysis: edge cases, data drift checks, reproducibility scripts.
- Iteration 5: Packaging + report: exportable model, usage guide, ethical considerations, final plots.

Systems/IoT/Embedded
- Iteration 1: Board bring-up and sensor read with mock; logging; unit tests on host.
- Iteration 2: Basic control loop; integration test harness; failure handling.
- Iteration 3: Telemetry to host service; simple dashboard; latency/throughput measurement.
- Iteration 4: Power/perf tuning; debouncing; watchdog; memory footprint check.
- Iteration 5: Enclosure/UX and deployment checklist; runbook.

Research/Algorithmic prototype
- Iteration 1: Reference implementation on small inputs; unit tests; baseline complexity measurement.
- Iteration 2: Correctness on edge cases; input validation; benchmark harness.
- Iteration 3: Optimization attempt; empirical analysis with plots.
- Iteration 4: Comparative evaluation vs. baseline; discussion of trade-offs.
- Iteration 5: Reproducible artifact (data/code/scripts), write-up draft aligned to course outcomes.

### Role rotation

Rotation guidance
- Leads coordinate but still contribute code. Pair programming encouraged for complex tasks.
- Reviewers should not be in the same focus role for that iteration to broaden perspectives.
- Use "co-authored-by" in commits for pair/mob sessions to capture contributions.

## Policies (replace meeting minutes)

- Weekly Status Report (team-level GitHub issue) includes: sprint goal/scope; done items with PR/issue links; release tag; CI status; tests/coverage; risks/blocks; next goal; individual contributions (PRs/reviews/hours).
- PR rules: linked issue and acceptance criteria; tests+docs; CI green; ≥1 reviewer; small/focused PRs; co-authored-by trailers for pair/mob.
- Contribution tracking: evaluated via authored PRs, meaningful reviews, commits tied to issues, and demo attribution.
- Automate as much as possible
- Week 16: Project Initial Draft
- Week 17: final v1.0 release, poster, handoff

## Instructor/TA
- Before lab: scan PRs/releases/CI and Status Report issue
- In lab: demos, spot checks, risk/quality Q&A
- After lab: comment on the Status Report with approval or change requests

Notes: Labs are protected team time; lectures remain lighter-touch and supportive of the above focuses.