## Wiki Purpose

- The user's personal knowledge base on "The re-emergent role of the Design Engineer in the age of AI".

## Wiki Architecture

`/raw` — a directory of source documents (ie. articles, papers, images, data files, etc.) curated by the user. These files are _immutable_ — the LLM reads them but _never modifies_ them. The user owns this layer entirely.

`/wiki` — a directory of HTML _topic pages_ (ie. summaries, synthesis, entities, concepts, comparisons, visualization, etc.). These files are _mutable_ — the LLM owns this layer entirely and is responsible for:
1. creating HTML pages and updating them when new /raw sources are injested.
2. maintaining cross-references across wiki pages.
3. keeping everything consistent.

`/outputs` — a directory of documents produced by the LLM from user queries.

`/skills` — a directory of repeatable instructions invoked by the user.

## Key Files

`index.html` — is a _content-oriented catalog of everything in the wiki_.
- Each _topic page_ in the wiki is represented here as a short `listing` (ie. title, one-line summary, hyperlink).
- Each `listing` is organized into categories (entities, concepts, sources, etc.) identified, created and maintained by the LLM.

`log.html` — is an append-only, _chronological record of what happened and when_.
- Naming convention: `[YYYY-MM-DD] | Topic Title`
- The purpose of the log is to enable the LLM to easily parse the records with simple unix commands (ie. `grep`).
