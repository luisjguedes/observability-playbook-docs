# Style guide (based on Microsoft Writing Style)

This repo follows a concise, customer-focused style aligned with Microsoft’s guidance:
https://learn.microsoft.com/en-us/style-guide/welcome/

This file is a practical “working standard” for contributors. It doesn't copy the Microsoft guide, it applies the same principles in a repo-friendly way.

---

## Core principles

### Write for scanning
- Put the **goal** first.
- Use short sections with meaningful headings.
- Keep paragraphs under ~4 lines when possible.

### Be clear and specific
- Prefer concrete verbs over abstract language.
- Prefer exact outcomes over vague claims.

✅ **Good:** “Returns `202 Accepted` when the event is queued.”  
❌ **Avoid:** “Returns a successful response.”

### Be customer-first
- Address the reader as **you**.
- Describe the product/system as **we** only when needed (and consistently).

---

## Voice and tone

### Use a neutral, professional tone
- Helpful, direct, and calm.
- Avoid hype and marketing language.

✅ “This endpoint supports idempotent retries.”  
❌ “This endpoint is super powerful and easy to use.”

### Use active voice
✅ “The API returns a request ID.”  
❌ “A request ID is returned.”

---

## Grammar and mechanics

### Use sentence case for headings
✅ “Send your first event”  
❌ “Send Your First Event”

### Use present tense
✅ “The API returns…”  
❌ “The API will return…”

### Avoid filler words
Avoid: *just, simply, basically, obviously, clearly, very, easy, quickly, in order to*.

✅ “Run `mkdocs serve`.”  
❌ “Simply run `mkdocs serve`.”

### Use consistent capitalization
- **API**, **URL**, **ID**, **JSON**, **YAML**
- **GitHub**, **MkDocs**, **OpenAPI**

---

## Content patterns (required)

### Concepts
Concept pages explain **what** and **why**.
Include:
- Definition
- Mental model
- When to use / when not to use
- One simple example

### How-to guides
How-to pages explain **how** to do a task.
Use this structure:
1. **Goal**
2. **Prerequisites**
3. **Steps**
4. **Expected result**
5. **Troubleshooting links** (if relevant)

### Reference
Reference pages are **complete and precise**.
Include:
- Endpoint summary table
- Auth requirements
- Headers
- Request fields (table)
- Responses (codes + error shape)
- Copy/paste examples

### Troubleshooting
Troubleshooting pages focus on symptoms and fixes.
Use:
- **Symptom**
- **Likely cause**
- **How to confirm**
- **Fix**
- **Prevention**

---

## API writing rules

### Use consistent status code meaning
- `200 OK`: successful read
- `201 Created`: created new resource
- `202 Accepted`: accepted for processing (async)
- `400 Bad Request`: validation error
- `401 Unauthorized`: missing/invalid auth
- `403 Forbidden`: authenticated but not allowed
- `404 Not Found`: unknown resource
- `409 Conflict`: state conflict / duplicate
- `429 Too Many Requests`: rate limited
- `500 Internal Server Error`: unexpected failure

### Always show examples in code fences
Use:
- ```http for requests/responses
- ```json for JSON payloads
- ```bash for curl commands

### Don’t hide required info
If an endpoint requires:
- token → state it
- idempotency → state it
- rate limits → state expected behavior

---

## Word list (preferred terms)

Use these terms consistently:

- **sign in** (verb), **sign-in** (noun/adjective)
- **set up** (verb), **setup** (noun)
- **run** a command (not “execute” unless needed)
- **select** (UI), **choose** (decision)
- **enter** (typed input), **type** (informal acceptable)
- **parameter** (API), **setting** (configuration)

---

## Accessibility and inclusivity

- Avoid idioms and sarcasm.
- Avoid terms like “easy,” “simple,” “trivial.”
- Prefer: “This takes about 2 minutes” or “This requires X.”

---

## Quick checklist (before merging)

- Headings are sentence case
- Steps are numbered and start with a verb
- Examples are copy/pasteable
- Terminology is consistent
- No filler words or hype
- Links to next steps / troubleshooting exist where helpful
