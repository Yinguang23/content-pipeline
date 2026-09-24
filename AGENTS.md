# Content pipeline instructions

All paths below are relative to the repository root.

Before any content work, always read `/workflow/README.md` completely. Treat it as the canonical creative instruction source, including title selection, caption style, output format, and quality checks. Do not recreate or duplicate its Chinese creative instructions here. Follow explicit user overrides for the current request.

Whenever a new English Caption idea is created or added:

1. Read both content files. Assign the next sequential TAB number: one greater than the highest numeric TAB in either file, or 1 if none exist. Ignore template placeholders. Preserve an already assigned unique TAB when processing an existing entry.
2. Append the idea to `/content/english-caption.md` using the exact `TAB:`, `STATUS: NEW`, `TOPIC:`, `CORE IDEA:`, `ENGLISH TITLE:`, `ENGLISH CAPTION:`, and `NOTES:` field structure from the workflow. Never delete or overwrite earlier entries.
3. Immediately process that same TAB using `/workflow/README.md`. Generate exactly 20 Chinese title ideas, select the strongest 3, write the long paragraph-style Chinese RedNote caption, and add relevant RedNote hashtags.
4. Append the completed package to `/content/chinese-rednote.md` in TAB order, preserving the same TAB number and marking the result `STATUS: PROCESSED`. Use the workflow's display heading and explicit `TAB: [number]` completion record. Keep the English source intact; the Chinese completion record determines whether it has been processed.
5. Before generating anything, check the Chinese output for that TAB's completed package. Never regenerate an already processed TAB unless the user explicitly requests a revision. Never alter existing processed content during ordinary appends. Do not reprocess older entries merely because their English source still says `STATUS: NEW`.
6. Run the workflow's final quality check, verify that earlier content is preserved, and commit and push all resulting changes to the existing content-processing pull request's branch. Follow the workflow's English-entry and completed-output commit sequence. Inspect open PRs before choosing the branch; if no content-processing PR exists, create one. Do not merge the PR unless asked.

Process only newly added entries during normal operation, plus any existing TAB the user explicitly asks to process or revise. An explicit English-only request defers Chinese processing until the user authorizes it.
