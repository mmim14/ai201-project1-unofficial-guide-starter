# Project 1 Planning: The Unofficial Guide

> Write this document before you write any pipeline code.
> Your spec and architecture diagram are what you'll use to direct AI tools (Claude, Copilot, etc.) to generate your implementation — the more specific they are, the more useful the generated code will be.
> Update the Retrieval Approach and Chunking Strategy sections if you change your approach during implementation.
> Update this file before starting any stretch features.

---

## Domain

<!-- What domain did you choose? Why is this knowledge valuable and hard to find through official channels? -->
I'm choosing the domain to be course and professor reviews at CUNY Baruch College for mathematics courses. It will include more details like worklaod (hours per week), how to prepare for exams, etc. Rate My Professors don't have details about the course and often times students have to hunt down other students who took the classes before to know more details, but that can be difficult. Having details about how to be successful in the specific course sets students for success. 

---

## Documents

<!-- List your specific sources: URLs, subreddit names, forum threads, or file descriptions.
     Aim for at least 10 sources that together cover different subtopics or perspectives within your domain. -->

| # | Source | Type | URL or file path |
|---|--------|------|-----------------|
| 1 | Baruch Math Course Catalog|pdf document |".\MATH-BAR-2026-01-13-20-37-18.pdf" |
| 2 | Coursicle Course Reviews | URL | https://www.coursicle.com/baruchcuny/courses/MTH/|
| 3 | Reddit (Baruch subreddit)| URL | https://www.reddit.com/r/Baruch/|
| 4 | Rate My Professors (Professor Arthur Apter)| URL | https://www.ratemyprofessors.com/ | https://www.ratemyprofessors.com/professor/206015
| 5 | Rate My Professor (Professor Jonathan Engel)| URL | https://www.ratemyprofessors.com/search/professors/222?q=Jonathan%20Engel |
| 6 | Rate My Professor (Professor Louis-Pierre Arguin)| URL | https://www.ratemyprofessors.com/professor/1959315 |
| 7 | Rate My Professor (Professor Ivan Matic) | URL | https://www.ratemyprofessors.com/professor/1855876 |
| 8 | Rate My Professor (Professor Peter Gregory) | URL | https://www.ratemyprofessors.com/professor/286765
| 9 | Rate My Professor (Professor Warren Gordon) | URL| https://www.ratemyprofessors.com/professor/227325 |
| 10 | Rate My Professor (Professor Miriam Hausman) | URL | https://www.ratemyprofessors.com/professor/275741 |

---

## Chunking Strategy

<!-- How will you split documents into chunks?
     State your chunk size (in tokens or characters), overlap size, and explain why those
     numbers fit the structure of your documents.
     A review-heavy corpus warrants different chunking than a long FAQ. -->

**Chunk size:**
I have multiple documents of various types. I would chunk the catalog by page and reviews on Rate My Professor and reddit post by itself. 

**Overlap:**

**Reasoning:**
The pages in the catalog is fairly split into pages. Reviews are best represented in the whole chunk than cutting it off. 

---

## Retrieval Approach

<!-- Which embedding model are you using (e.g., all-MiniLM-L6-v2 via sentence-transformers)?
     How many chunks will you retrieve per query (top-k)?
     If you were deploying this for real users and cost wasn't a constraint, what tradeoffs
     would you weigh in choosing a different embedding model — context length, multilingual
     support, accuracy on domain-specific text, latency? -->

**Embedding model:**

**Top-k:**

**Production tradeoff reflection:**

---

## Evaluation Plan

<!-- List your 5 test questions with their expected correct answers.
     Questions should be specific enough that you can judge whether the system's response
     is right or wrong. "What are good dining halls?" is too vague.
     "What do students say about wait times at [dining hall name] during lunch?" is testable. -->

| # | Question | Expected answer |
|---|----------|-----------------|
| 1 | | |
| 2 | | |
| 3 | | |
| 4 | | |
| 5 | | |

---

## Anticipated Challenges

<!-- What could go wrong? Name at least two specific risks with reasoning.
     Consider: noisy or inconsistent documents, missing source attribution, off-topic
     retrieval, chunks that split key information across boundaries. -->

1.

2.

---

## Architecture

<!-- Draw a diagram of your pipeline showing the five stages:
     Document Ingestion → Chunking → Embedding + Vector Store → Retrieval → Generation
     Label each stage with the tool or library you're using.
     You can use ASCII art, a Mermaid diagram, or embed a sketch as an image.
     You'll use this diagram as context when prompting AI tools to implement each stage. -->

---

## AI Tool Plan

<!-- For each part of the pipeline below, describe:
     - Which AI tool you plan to use (Claude, Copilot, ChatGPT, etc.)
     - What you'll give it as input (which sections of this planning.md, which requirements)
     - What you expect it to produce
     - How you'll verify the output matches your spec

     "I'll use AI to help me code" is not a plan.
     "I'll give Claude my Chunking Strategy section and ask it to implement chunk_text()
     with my specified chunk size and overlap" is a plan. -->

**Milestone 3 — Ingestion and chunking:**

**Milestone 4 — Embedding and retrieval:**

**Milestone 5 — Generation and interface:**
