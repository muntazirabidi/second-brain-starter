---
name: ask
description: Answer a question from the user's own wiki, citing the pages used. Use when the user asks what they know, what their sources say, what they have read about something, or any question about the subject this brain follows.
argument-hint: "<question>"
---

Question: $ARGUMENTS

1. Start from `wiki/index.md`. Open every topic and source page that looks relevant and read them in full.
2. Answer in a few short paragraphs. After each claim, link the page it came from, for example ([[prompt-caching]]).
3. If the wiki does not cover it, say "Your wiki doesn't cover this yet", suggest what to capture, and only then add general knowledge, clearly labelled.
4. If the answer pulled several pages together in a useful way, offer to save it as a new topic page.
