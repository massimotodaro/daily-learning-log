# Daily Learning Log

This repository is a durable record of what I learn, build, test, and improve each day.
The aim is consistent, honest progress: every entry should preserve something genuinely
useful to my future self, even when the day's lesson is small.

## Daily rules

1. Record one real learning, experiment, correction, or completed improvement.
2. Describe the result in my own words; do not paste material without attribution.
3. Prefer evidence over claims: include a command, test result, source, example, or link
   when it makes the learning reproducible.
4. Separate confirmed facts from assumptions, opinions, and open questions.
5. Never include secrets, credentials, tokens, private keys, connection strings, personal
   data, confidential business information, or private material from another repository.
6. Do not manufacture activity, backdate entries, or claim work that was not performed.
7. Keep each commit focused on that day's genuine addition or correction.
8. Correct mistakes openly in a later entry instead of silently rewriting history.
9. Credit collaborators and original sources when their work informed the entry.
10. A day with a failed experiment still counts when the failure and lesson are recorded
    accurately.

## Repository structure

```text
daily-learning-log/
├── Master.md
├── Index.md
├── templates/
│   └── Daily.md
└── entries/
    └── YYYY/
        └── YYYY-MM-DD.md
```

- `Master.md` owns the rules, areas, identifiers, and formats.
- `Index.md` is the navigation surface and contains one row per lesson.
- `templates/Daily.md` is the reusable entry template.
- `entries/YYYY/YYYY-MM-DD.md` contains all lessons recorded for one calendar day.

## Lesson identifiers and indexing

Every distinct lesson receives a permanent identifier in this form:

```text
DL-YYYY-MM-DD-NN
```

`NN` starts at `01` each day and increases in the order the lessons appear. Do not reuse
or renumber an identifier after publication. Corrections should link to the original
lesson and explain what changed.

Every lesson must have its own row in `Index.md`, including:

- its permanent identifier;
- date;
- descriptive title linked to its stable anchor;
- learning areas; and
- concise lowercase tags.

When adding or correcting an entry, update `Index.md` in the same commit. Topic-specific
indexes should be introduced only when the main index becomes difficult to navigate.

## Learning areas

Use one or more of these labels in each daily entry.

### Software engineering

- Programming languages and implementation techniques
- Architecture, APIs, data modelling, and system design
- Refactoring, maintainability, and technical debt
- Testing, debugging, performance, and reliability

### AI and agent systems

- Models, prompting, context, tools, and agent harnesses
- Evaluations, guardrails, observability, and human oversight
- Retrieval, embeddings, inference, and model integration
- Responsible AI, limitations, and failure modes

### Cloud and delivery

- Linux, containers, networking, and infrastructure
- CI/CD, GitHub, deployments, and release engineering
- Cloud platforms, databases, storage, and monitoring
- Cost, scaling, availability, recovery, and operations

### Security and privacy

- Authentication, authorization, and least privilege
- Secure coding, threat modelling, and vulnerability remediation
- Data protection, encryption, retention, and auditability
- Supply-chain and dependency security

### Product and design

- Product strategy, requirements, and prioritisation
- User research, workflows, accessibility, and UI/UX
- Metrics, experimentation, and decision-making
- Documentation and communication

### Education and domain knowledge

- Teaching, learning science, assessment, and curriculum
- School operations, safeguarding, and inclusion
- UK education policy and responsible educational technology
- Domain terminology and stakeholder needs

### Business and leadership

- Entrepreneurship, planning, finance, and commercial thinking
- Legal, procurement, compliance, and provider assessment
- Leadership, collaboration, negotiation, and feedback
- Personal productivity and professional development

### Tools and workflow

- Git, editors, terminals, automation, and developer tooling
- Research methods and information management
- Repeatable processes, checklists, and templates
- Workflow improvements and lessons from mistakes

## Daily entry format

Start from [`templates/Daily.md`](templates/Daily.md). A daily file may contain one or
more lessons, but every lesson must independently include:

- permanent identifier and descriptive title;
- areas and tags;
- what I learned;
- what I did;
- evidence or example;
- why it matters;
- open questions;
- next step; and
- sources.

If an entry is written after the date it describes, place a retrospective notice directly
below the date heading and retain the real Git commit timestamp.

## Commit convention

Use a concise commit subject that describes the learning rather than the contribution
streak. Recommended forms:

```text
learn: document <topic>
build: add <experiment>
test: record <result>
fix: correct <previous understanding>
reflect: capture <lesson>
```

The contribution graph is a side effect. The lasting value is a searchable, trustworthy
record of progress.
