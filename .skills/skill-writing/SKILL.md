---
name: skill-writing
description: Create or update local workspace skills under .skills. Use when the user asks to design, write, revise, organize, or discuss Codex skills for this agentic programming root, especially skills stored as .skills/<skill-name>/SKILL.md.
---

# Skill Writing

Use the installed system `skill-creator` skill first. Read its `SKILL.md` completely before creating or revising a local skill, then apply the local conventions below.

## Local Conventions

- Store local skills under `.skills/<skill-name>/SKILL.md`.
- Name skill folders with lowercase letters, digits, and hyphens only.
- Keep the folder name and frontmatter `name` identical.
- Use only `name` and `description` in YAML frontmatter.
- Write `description` as the trigger surface: include what the skill does and when Codex should use it.
- Keep `SKILL.md` concise and procedural.
- Add optional `references/`, `scripts/`, or `assets/` folders only when the skill genuinely needs them.
- Do not add extra docs such as `README.md`, installation guides, changelogs, or quick references inside skill folders.
- Add or update a quick trigger direction for every local skill in the `## Skills` section of `AGENTS.md`.

## Workflow

1. Clarify the concrete tasks or prompts that should trigger the skill.
2. Decide whether a new skill is warranted, or whether `AGENTS.md` is the better home for broad root instructions.
3. Draft the skill folder at `.skills/<skill-name>/SKILL.md`.
4. Keep reusable details out of the main skill body unless they are essential on every use.
5. Add or update the matching `AGENTS.md` `## Skills` bullet in this form: `- When <trigger>, read and follow \`.skills/<skill-name>/SKILL.md\`.`
6. Validate the skill against a few realistic trigger prompts and revise the description if triggering would be ambiguous.
7. Update other `AGENTS.md` guidance only when root-level discovery or policy changes are needed.

## Quality Bar

A local skill is ready when another Codex instance can read only its metadata and know when to load it, then read its `SKILL.md` and execute the workflow without needing hidden context from the original discussion.
