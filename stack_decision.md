# Stack Decision

**Industry / use case:** HR/Career services - personalized interview preparation for job seekers

**Primary stack:** n8n

**Team:** Julia Antunes and Roodabeh Seif  

## Why n8n fits this problem

Our workflow is mostly a predictable sequence: collect the inputs, research the company, retrieve relevant context, compare the role with the candidate's background, and assemble a one-page report. n8n suits this shape because the trigger, API connections, branching, and error paths can be built and inspected in one visual workflow. Its form trigger gives job seekers a simple way to submit their details without us building a separate interface. The visual workflow also makes it easy for both team members to explain the architecture and show each step during the demo. With only five days, n8n lets us spend more time on report quality and reliability than on application plumbing.

## Why LangGraph is out of scope for the MVP

LangGraph gives more control over state, cycles, and multi-step agent reasoning. The MVP does not need open-ended planning or a complex reasoning loop, because the research steps and report structure are known in advance. Using it here would add code and complexity without a clear benefit for the user. We would reconsider LangGraph if a later version needed adaptive research, repeated self-correction, or long-running state across several interview rounds.

## Trade-offs

| Criterion | n8n | LangGraph | Decision for the MVP |
|---|---|---|---|
| Time to demo | Faster for a linear flow with API calls | Requires more setup and code | n8n |
| Control over agent logic | Moderate | High | Sufficient in n8n |
| Operations integration | Built-in trigger, HTTP, and AI nodes | Must be coded or added | n8n |
| Branching and failure paths | Visible in the workflow | Flexible, defined in code | n8n |
| Explainability in the demo | Each step is visible | Requires a graph walkthrough | n8n |

## Known limitations of this choice

- Complex logic can become difficult to read in a large visual workflow, so we will keep it to clearly named sections.
- Version control is less natural than with Python, so we will export the workflow JSON to GitHub after each meaningful change.
- Testing individual steps is less rigorous than unit testing code, so we will test each tool separately and run at least two full sample targets.

## Planned tools

These are proposed for Day 1 and must be confirmed by testing the API keys.

| Capability | Candidate | Purpose |
|---|---|---|
| Web search | Tavily | Company background and job-page research |
| News | GNews or NewsAPI | Two or three recent, relevant news items |
| Public developer data | GitHub REST API | Public repositories and project evidence |
| Retrieval | Pinecone | Grounding in the CV and interview-preparation guidance |
| LLM | OpenAI or Anthropic | Analysis and report writing |

The candidate provides their CV directly. The MVP does not scrape LinkedIn or any private personal data.
