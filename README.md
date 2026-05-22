# claude-marketplace

A marketplace of Claude Code skills by Thibault Duponchelle.

## Available skills

| Name | Description |
|------|-------------|
| `42` | Replies 42 to any question |

## Installation

### 1. Add this marketplace

```
/plugin marketplace add thibaultduponchelle/claude-marketplace
```

### 2. Install a skill

```
/plugin install 42
```

### 3. Reload plugins

```
/reload-plugins
```

### 4. Use the skill

```
/42
```

## Adding your own skills

Each skill lives under `skills/<skill-name>/SKILL.md` and is declared in `.claude-plugin/marketplace.json`.

**SKILL.md** format:

```markdown
---
name: my-skill
description: What this skill does
---

Instructions for Claude to follow when this skill is invoked.
```

**marketplace.json** entry:

```json
{
  "name": "my-skill",
  "source": "./skills/my-skill",
  "description": "What this skill does"
}
```
