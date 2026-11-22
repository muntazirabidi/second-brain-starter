# Second Brain

My personal knowledge base, following Andrej Karpathy's "LLM wiki" idea. I collect what I read and hear. You, the agent, read it, file it and keep the wiki tidy. I never write the wiki myself.

Read `profile.md` first. It says who I am, which subject this brain follows (AI, or my own field), and how I like answers.

## Folders

- `raw/`: what I collect. Articles, PDFs, links, meeting notes, my own thoughts. One file each, never edited after saving, except the `status:` line.
- `wiki/`: what I know. You write and maintain it.
  - `wiki/index.md`: every wiki page, one line each, grouped by type. Update it whenever a page is added.
  - `wiki/log.md`: one entry for every change, newest at the bottom: `## [YYYY-MM-DD] action | title`.
  - `wiki/sources/`: one summary page per item in `raw/`.
  - `wiki/topics/`: one page per idea, method, person, company or tool. These are the pages that grow over time.

## How pages are written

- Plain Markdown. File names in lowercase with hyphens, for example `prompt-caching.md`.
- Link pages with `[[page-name]]`. Obsidian, if I install it, shows these as a map.
- Every fact on a topic page says which source page it came from.
- If a new source disagrees with an existing page, keep both claims with their dates and mark it **Disagreement**. Never quietly overwrite.
- Update an existing topic page rather than creating a near duplicate.

## Skills

| Type | What happens |
|---|---|
| `/capture <link, file or pasted text>` | saved into `raw/`, nothing else changes |
| `/ingest <raw file>` | read in full, two questions for me, then source page, topic pages, index and log |
| `/ask <question>` | answered only from the wiki, with links to the pages used |
| `/today` | what is waiting, what I added recently, one suggestion |
| `/weekly` | the week in review, three quiz questions, then save a version with git |

## Rules

- Answer from the wiki first. If it does not cover something, say so clearly, then label anything from general knowledge as such.
- Client or patient material: use made up names unless I say otherwise. Never put passwords, keys or bank details anywhere in this folder.
- Never delete anything in `raw/`. Ask before deleting a wiki page.
- Plain British English, short sentences.
- After each session that changed things, offer to save a version with git.
