# Contributing to Claude Code Skills

Thank you for your interest in contributing! This document provides guidelines for contributing to this repository.

## How to Contribute

### Reporting Issues

If you find a bug or have a suggestion:

1. Check if an issue already exists
2. If not, create a new issue with a clear description
3. Include examples or use cases if applicable

### Submitting a New Skill

1. Fork the repository
2. Create a new branch: `git checkout -b add-skill-<skill-name>`
3. Create your skill following the structure below
4. Test your skill locally
5. Submit a pull request

## Skill Structure

Each skill must follow this structure:

```
<skill-name>/
└── SKILL.md
```

### SKILL.md Format

```markdown
---
name: skill-name
version: 1.0.0
description: Brief description of what the skill does
triggers:
  - trigger1
  - trigger2
---

# Skill Title

Content and instructions for the skill...
```

### YAML Front Matter Fields

| Field | Required | Description |
|-------|----------|-------------|
| `name` | Yes | Unique identifier for the skill (kebab-case) |
| `version` | Yes | Semantic version (e.g., 1.0.0) |
| `description` | Yes | Brief description of the skill's purpose |
| `triggers` | Yes | List of keywords that invoke this skill |

## Guidelines

### Naming Conventions

- Skill names should be lowercase, kebab-case (e.g., `pr-review`, `code-refactor`)
- Names should be descriptive but concise

### Content Guidelines

- Write clear, actionable instructions
- Use markdown formatting for readability
- Include examples when helpful
- Keep skills focused on a single purpose

### Language

- Skills can be written in any language
- Prefer the language most natural for the skill's target audience

## Pull Request Process

1. Ensure your skill follows the structure and guidelines above
2. Update the README.md to include your skill in the "Available Skills" table
3. Write a clear PR description explaining the skill's purpose
4. Wait for review and address any feedback

## Code of Conduct

- Be respectful and constructive
- Welcome newcomers
- Focus on collaboration

## Questions?

If you have questions, feel free to open an issue for discussion.
