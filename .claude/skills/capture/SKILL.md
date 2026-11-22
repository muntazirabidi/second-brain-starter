---
name: capture
description: Save a link, file, pasted text or quick thought into raw/ exactly as it is, with a short header, without changing the wiki. Use when the user says capture, save this, remember this, add this, here is an article, or pastes something to keep.
argument-hint: "<link | file path | pasted text>"
---

Item to capture: $ARGUMENTS

1. If it is a link, read the page. If it is a file, read it. If it is pasted text or a thought, use it as given.
2. Save it as `raw/YYYY-MM-DD-short-title.md` (today's date, a few words of title in lowercase with hyphens). For a PDF or other file, copy it into `raw/` and also write this `.md` file beside it with the header and a note of the file name.
3. Start the file with this header, then the full text:

   ```
   title:
   source: (the link, the file name, or "my own note")
   captured: YYYY-MM-DD
   why: (one line on why it matters, based on profile.md)
   status: new
   ```

4. Do not summarise and do not touch `wiki/`. That is /ingest.
5. Reply in two lines: what was saved, and "Run /ingest raw/<file> when you are ready."
