# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a collection of reusable skills for Claude Code agents. Skills are modular prompts that extend Claude Code's capabilities, triggered by specific keywords or `/skill-name` commands.

## Architecture

```
skills/
├── <skill-name>/
│   └── SKILL.md       # Skill definition with YAML front matter + markdown content
├── README.md
└── CONTRIBUTING.md
```

### Skill File Format (SKILL.md)

Each skill is a markdown file with YAML front matter:

```markdown
---
name: skill-name          # Required: kebab-case identifier
version: 1.0.0            # Required: semantic version
description: Brief desc   # Required: what the skill does
triggers:                 # Required: keywords that invoke the skill
  - trigger1
  - trigger2
---

# Skill content in markdown...
```

## Adding a New Skill

1. Create directory: `<skill-name>/`
2. Create `SKILL.md` with required YAML fields (name, version, description, triggers)
3. Update README.md "Available Skills" table
4. Branch naming: `add-skill-<skill-name>`

## Conventions

- Skill names: lowercase, kebab-case (e.g., `pr-review`, `code-refactor`)
- Skills can be written in any language appropriate for the target audience
- Keep skills focused on a single purpose
