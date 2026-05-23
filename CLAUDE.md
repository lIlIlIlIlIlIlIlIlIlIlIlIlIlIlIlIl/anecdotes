# Anecdotes — Claude Code Instructions

## Language

Always respond in **French**, regardless of the language used in the prompt.

Never use em dashes (—) in any written text (comments, documentation, env files), except in the `#` title line of a `.md` file: use a comma or parentheses instead.

Never use `---` horizontal rules as section separators in Markdown files; use headings (`##`, `###`) to structure content.

Write all anecdotes in **French**.

Terms from other languages (English, Latin, Portuguese, etc.) may appear within entries, but the main sentence must always be in French.

## Project Structure

| File           | Role                                                    |
| -------------- | ------------------------------------------------------- |
| `ANECDOTES.md` | Main file, all anecdotes hierarchically sorted          |
| `CLAUDE.md`    | Contribution rules (language, sorting, style, accuracy) |

`ANECDOTES.md` uses four heading levels with systematic emojis:

- `#`: Document title (includes entry count)
- `##`: Major thematic category
- `###`: Subcategory
- `####`: Sub-subcategory (optional)
- `-`: Individual anecdote entries, alphabetically sorted within each section

## Key Invariants

- **Alphabetical order**: all entries must be sorted alphabetically at every level: categories (`##`), subcategories (`###`/`####`), and individual entries
- **Epistemic hedging**: if a fact is uncertain, use the epistemic conditional ("aurait", "serait") or hedged phrasing ("selon", "environ") rather than stating it as certain
- **Gate on uncertainty**: if a fact cannot be confirmed, do not add the anecdote, or explicitly flag the uncertainty to the user before adding it
- **Restore order**: when adding or editing any entry, verify and restore alphabetical order in the affected section
- **Sort key**: sort on the full first word of the entry, article included (e.g., "La" < "Le" < "Les" < "Un"; "L'" sorts before "La" because the apostrophe character precedes letters)
- **Verified facts only**: every anecdote must be 100% true and verified; never invent, extrapolate, or approximate beyond what is documented

## Content Quality Standards

These rules apply to **every file, every change**, without exception.

### Formatting

- **Quotes**: always use straight double quotes `"` for highlighting terms within anecdotes, never French guillemets `«»`

### Style

- **Figures**: precise figures with ranges where appropriate
- **One sentence**: one sentence per anecdote, concise and synthetic; include only the most essential elements
- **Structure**: common form is main fact + causal explanation (`, car`, `: `, `;`)
- **Tone**: encyclopedic, neutral, assertive; always prefer the simplest and most professional phrasing
