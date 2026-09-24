# Content pipeline instructions

All paths below are relative to the repository root.

Before any content work, always read `/workflow/README.md` completely. It is the canonical creative instruction source. Follow its PRIMARY SOURCE — SCRIPT 3 section for sourcing and processing; that section and the user's current instructions supersede the older English-queue and pull-request behavior later in the workflow. Do not recreate its Chinese creative instructions here.

## Source and processing

1. Read the Script 3 Google Doc directly using the link in `/workflow/README.md`. Script 3 is the canonical source. `/content/english-caption.md` and `/content/chinese-rednote.md` are outputs and processing history, never the source of new scripts.
2. Identify new or substantially changed scripts/tabs. Treat Tabs 1–64 as the historical baseline unless the user explicitly says otherwise. Read each eligible script in full and preserve its original Script 3 TAB number; do not assign a new sequential number from the output files.
3. Compare against recorded source versions and processing history. Skip unchanged processed scripts. A substantial change affects the core idea, claims, examples, argument, or hook; formatting and minor wording changes alone do not require regeneration. If source access or comparison evidence is missing, report the limitation rather than treating output text as the source or claiming a change was detected.
4. Generate the complete English package first, following the canonical workflow's source/output fields and applicable user instructions. Then generate the complete Chinese RedNote package using the workflow: exactly 20 title ideas, the strongest 3, a long paragraph-style Chinese caption, and relevant hashtags.
5. Append the English package to `/content/english-caption.md` and the Chinese package to `/content/chinese-rednote.md`. Preserve existing content. For a substantially changed script, append a clearly identified revision under the same source TAB number instead of overwriting prior output.
6. Record the source document/tab identity and enough source-version or snapshot information to compare future changes. Mark the completed result `STATUS: PROCESSED`. Do not regenerate unchanged processed TABs unless explicitly requested.
7. Run the workflow's quality checks and verify that both outputs are saved and previous content is preserved.

## Git workflow

Work on the latest `main`. Commit and push completed outputs and associated processing records directly to `main`. Do not create or update a pull request unless the user explicitly requests one. Do not force-push or discard unrelated changes. If direct pushing is blocked, report the actual blocker rather than creating a PR automatically.

Explicit user instructions, including requests to defer one language or revise a historical TAB, override the normal behavior for that request.
