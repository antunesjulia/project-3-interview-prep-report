# Interview Prep Report Template

**Reader:** A job seeker with an interview coming up

**Useful means:** In five minutes, the reader knows what to say about the company, which of their own examples to use, what to prepare, and which questions to expect.

**Length:** One page, about 500 words

---

# Interview Prep: {{role_title}} at {{company_name}}

*Prepared for {{candidate_name}} on {{date}}*

## 1. Company background (max 50 words)

{{what the company does, who it serves, and its size or market position when sourced}} [source]

## 2. Recent relevant news (2-3 items, max 25 words each)

- **{{date}}:** {{what happened and why it matters for this role}} [source]

If no relevant news is found, write: "No relevant news found in the last 12 months."

## 3. Role requirements (max 5 bullets, 12 words each)

- {{requirement, marked Must-have or Nice-to-have based on the job posting}}

## 4. Your match (3 rows, max 30 words each)

| Requirement | Your evidence | Strength |
|---|---|---|
| {{requirement}} | {{specific experience from the CV or GitHub}} | Strong / Partial |

## 5. Projects to highlight (2 projects, max 35 words each)

- **{{project name}}:** {{what to say about it and which requirement it proves}}

## 6. Skill gaps to address (max 3, 25 words each)

- **{{gap}}:** {{concrete preparation step before the interview}}

## 7. Likely interview questions (5, max 15 words each)

1. {{question tied to the role, company, or candidate's background}}

---

## Quality rules

| Rule | Check |
|---|---|
| Grounded company facts | Sections 1 and 2 include a source link for every factual claim |
| No invented experience | Sections 4 and 5 use only the CV, the public GitHub profile, or text supplied by the candidate |
| Honest gaps | A requirement without evidence appears in section 6, not section 4 |
| Tailored questions | Each question refers to the role, company, or candidate's background |
| One page | The final report stays within about 500 words |
| Clear output | The report contains no raw API output, JSON, or placeholder text |

## Handling missing or failed inputs

| Situation | Behavior |
|---|---|
| Job link cannot be read | Ask for the job description text, and stop before generating a report |
| No CV or GitHub profile is provided | Ask for at least one source, and stop before generating a report |
| GitHub is unavailable, but a CV exists | Continue from the CV and note the missing source |
| News API fails or finds nothing | Retry once, then use the "no relevant news" message |
| Company research finds too little | State that public information is limited, and do not fill the gap with guesses |
