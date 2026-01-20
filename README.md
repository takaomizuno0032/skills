# Claude Code Skills

A collection of reusable skills for Claude Code agents, following Anthropic's official guidelines.

## Overview

This repository provides a curated set of skills that enhance Claude Code's capabilities. Skills are modular prompts that can be triggered by specific keywords or commands.

## Installation

Clone this repository to your local `.claude/skills` directory:

```bash
git clone git@github.com:takaomizuno0032/skills.git ~/.claude/skills
```

## Available Skills

| Skill | Description | Triggers |
|-------|-------------|----------|
| [pr-review](./pr-review/SKILL.md) | PR review checklist for code quality, security, testing, and documentation | `PR`, `review`, `pull request` |
| [pair-programming](./pair-programming/SKILL.md) | 対話型ペアプログラミング。実装前に複数案を提案し、議論を経て段階的に実装する | `pair`, `ペアプロ`, `相談`, `discuss` |

## Usage

Skills are automatically available in Claude Code. Use the trigger keywords to invoke a skill:

```
/pr-review
```

## Skill Structure

Each skill is defined in its own directory with a `SKILL.md` file:

```
skills/
├── README.md
├── CONTRIBUTING.md
└── <skill-name>/
    └── SKILL.md
```

The `SKILL.md` file contains:
- YAML front matter with metadata (name, version, description, triggers)
- Markdown content with the skill's instructions

## Roadmap

- Define an interface that supports Codex as well
- Add more community-contributed skills

## Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines.

## License

MIT License
