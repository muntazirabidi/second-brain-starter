---
name: ingest
description: Turn one file in raw/ into wiki knowledge. Read it in full, ask the user two questions, write a source page, create or update topic pages with links and citations, flag disagreements, then update the index and log. Use when the user says ingest, process this, file this, add it to the wiki, or after /capture.
argument-hint: "<raw/file>"
---

File to ingest: $ARGUMENTS (if empty, use the oldest file in `raw/` with `status: new`)

1. Read the file completely. Read `profile.md` and `wiki/index.md`.
2. Before writing anything, give the user three key points in plain words and ask two short questions: what surprised them, and how it connects to their work. Wait for the answers.
3. Write `wiki/sources/<same-name>.md`: title, source link, date, a five line summary, the key points, the user's answers under "My take", and links to the topic pages it touches.
4. For each important idea, method, person, company or tool:
   - If a topic page exists, add what is new under the right heading, with "(from [[source-page]])".
   - If not, create `wiki/topics/<name>.md` with a one line definition, what the source says, and links.
   - If it disagrees with what a page already says, keep both with dates and mark **Disagreement**.
5. Add any new pages to `wiki/index.md`. Add one entry to `wiki/log.md`.
6. Change the raw file's `status: new` to `status: ingested`. Change nothing else in it.
7. Reply with the pages created and updated, then offer: "Want three quick questions to check it stuck?"
