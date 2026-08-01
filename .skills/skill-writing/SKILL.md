---
name: skill-writing
description: Create or update local Codex skills under .skills. Use when designing, writing, revising, organizing, or discussing workspace skills.
---

# Skill Writing

Read and follow the installed system `skill-creator` skill first, then apply these local rules.

## Rules

- Store skills at `.skills/<skill-name>/SKILL.md`.
- Use lowercase letters, digits, and hyphens for skill names.
- Keep the folder name and frontmatter `name` identical.
- Use only `name` and `description` in YAML frontmatter.
- Make `description` the trigger surface: what the skill does and when to use it.
- Keep `SKILL.md` concise and procedural.
- Add `references/`, `scripts/`, or `assets/` only when needed.
- Do not add README-style docs inside skill folders.
- Add or update a matching `AGENTS.md` `## Skills` bullet: `- When <trigger>, read and follow \`.skills/<skill-name>/SKILL.md\`.`

## Workflow

1. Clarify the prompts or tasks that should trigger the skill.
2. Decide whether this belongs in a skill or in `AGENTS.md`.
3. Write or update `.skills/<skill-name>/SKILL.md`.
4. Run the `skill-creator` validator when available.
5. Test the description against realistic trigger prompts.
