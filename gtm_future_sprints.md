# Future Go-to-Market Sprints

These proposed sprints follow the MVP; they are not completed work. Validate
the targets as the team learns. The goal is to prove value with individual job
seekers, win an institutional pilot, then test whether organizations will pay.

**Current MVP:** An n8n workflow that turns a job posting and a candidate's
background into a grounded, one-page interview preparation report.

**Value proposition:** In five minutes, a job seeker knows what to say about
the company, which of their examples to use, what to prepare, and which questions
to expect.

## Summary

| | Sprint 1: Prove usefulness | Sprint 2: Institutional pilot | Sprint 3: Test willingness to pay |
|---|---|---|---|
| **Duration** | 3 weeks | 4 weeks | 4 weeks |
| **Audience** | Active job seekers | University career centers | Bootcamps and career coaches |
| **Channel** | LinkedIn, alumni, and bootcamp groups | Direct outreach and live demos | Referrals and career-coach networks |
| **Key deliverable** | Hosted beta and user feedback | Pilot offer and demo pack | Pricing and per-report plan |
| **Proposed success metric** | 20 reports; at least 70% rated useful | 1 agreed pilot | 5 paying partners |

## Before recruiting real users

The first sprint begins with a readiness check. Do not collect real CVs or
candidate information until the workflow is usable and the data-handling basics
are in place.

- Provide a stable hosted form and a clear privacy notice.
- Define how submitted CVs and other candidate data are retained and deleted.
- Review the terms of each API provider; confirm whether paid plans are required.
- Confirm that reports can be reviewed and delivered, and document how to handle
  common API and workflow failures.

If these conditions are not met, use the early Sprint 1 time to address them
before inviting participants.

## Sprint 1 — Prove usefulness with job seekers

**Goal:** Confirm that real job seekers find the report useful before an
upcoming interview.

**Target users:** People with an interview scheduled within the next upcoming weeks.

**Channel:** Personal LinkedIn posts and direct invitations through bootcamp
and alumni groups.

**Key deliverable:** A hosted beta with a simple form, privacy notice, and
short post-report survey.

**Activities:**

- Recruit participants and generate reports for real interviews.
- Observe where users struggle to provide a job description, CV, or GitHub
  profile.
- Ask users to rate usefulness, interview-question relevance, and confidence
  in sourced company facts.
- Track successful report delivery, completion time, missing inputs, and
  workflow failures.
- Review reports for required sections, usable source links, and unsupported
  claims about candidate experience.

**Proposed success metric:** 20 reports generated, with at least 70% rated
useful by users.

**Decision:** If usefulness is below 70%, improve the weakest report sections
or form steps and repeat the test before Sprint 2. Treat the target as a
hypothesis and record response counts alongside ratings.

**Deliverable:** Beta, feedback summary, and prioritized improvements.

## Sprint 2 — Win a first institutional pilot

**Goal:** Test whether career-services teams would offer the report to the
people they support.

**Target buyer:** Heads of university career centers; career advisers are the
day-to-day users.

**Channel:** Direct outreach to career centers, starting with universities
where the team has existing connections, followed by a live demo.

**Key deliverable:** A one-page pilot offer, a demo pack with sample reports
and Sprint 1 results, and a data-protection summary.

**Activities:**

- Share Sprint 1 evidence and demonstrate both the workflow and report.
- Test job-posting and candidate-input paths, including missing or unreadable
  inputs.
- Track report completion, source-link validity, report quality, and feedback
  from advisers and job seekers.
- Record objections and what a career center would need to run a pilot.

**Proposed success metric:** One pilot agreed with a career center.

**Decision:** If no center agrees after outreach, use the objections to revise
the offer or move directly to testing the Sprint 3 audience.

**Deliverable:** Pilot agreement or documented buyer feedback, plus updated
pilot materials.

## Sprint 3 — Test willingness to pay

**Goal:** Find out whether organizations that prepare people for interviews
will pay for reports.

**Target buyers:** Bootcamp career teams and independent career coaches.

**Channel:** Referrals from pilot contacts, alumni, and career-coach networks.

**Key deliverable:** A simple pricing page or offer, a per-report plan, and a
cost model that includes API usage.

**Activities:**

- Confirm API terms and paid plans needed for commercial use.
- Estimate delivery and support costs per report.
- Present a paid report package to potential partners and track conversions
  and objections.
- Keep operational monitoring and documented recovery steps for common
  workflow failures.

**Proposed success metric:** Three paying partners, each buying at least one
report package.

**Decision:** If fewer than three partners pay, compare objections about price
and value, then decide whether to change the buyer, offer, or pricing.

**Deliverable:** Pricing and cost findings, plus a decision on the next
commercial step.

## Out of scope for these sprints

- Multi-tenant accounts and production authentication.
- Paid advertising or a public self-serve launch.
- Adaptive, multi-round research with LangGraph.
- Persistent candidate profiles or interview-round history.

Revisit these if and when user or partner evidence shows a clear need.
