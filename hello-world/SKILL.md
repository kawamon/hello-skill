---
name: hello-world
description: A minimal "Hello World" sample skill for testing and learning. Use this skill when the user says "hello", asks for a greeting, or wants to test that skills are working correctly.
---

# Hello World Skill

A minimal sample skill that demonstrates the basic structure of a Claude Code skill. Use this as a starting point to understand how skills work or to verify your skill development environment.

## When to Use This Skill

Use this skill when:
- The user says "hello" or asks for a greeting
- The user wants to verify that skills are loaded and working
- The user is learning how to create new skills

## Core Behavior

When this skill is invoked, respond with a friendly greeting that includes:

1. A "Hello World!" message
2. Confirmation that the skill was loaded successfully
3. A brief summary of what this skill demonstrates

**Example response:**

```
Hello World! This skill is working correctly.

This is a sample skill that demonstrates:
- SKILL.md frontmatter (name, description)
- Structured sections (When to Use, Core Behavior, etc.)
- How Claude uses skill instructions to shape responses
```

## Skill Structure Reference

This skill follows the standard structure:

```
hello-skills/                     # Project root (separate from td-skills)
  .claude-plugin/
    marketplace.json              # Plugin registration
  hello-world/
    SKILL.md                      # This file - the skill definition
```

### Frontmatter Fields

| Field | Purpose | Example |
|-------|---------|---------|
| `name` | Unique skill identifier (lowercase-with-hyphens) | `hello-world` |
| `description` | When Claude should activate this skill | `"A minimal sample skill..."` |

### Recommended Sections

1. **When to Use This Skill** - Trigger conditions
2. **Core Principles / Core Behavior** - Main instructions for Claude
3. **Common Patterns** - Reusable examples
4. **Best Practices** - Guidelines
5. **Common Issues and Solutions** - Troubleshooting
6. **Related Skills** - Cross-references

## Creating Your Own Skill

To create a new skill based on this example:

1. Create a new folder: `your-skill-name/`
2. Add a `SKILL.md` with frontmatter (`name` and `description`)
3. Register it in `.claude-plugin/marketplace.json` の `skills` 配列に追加
4. Treasure Studio の `/plugin marketplace add <path>` で登録

## Resources

- [Claude Code Skills Documentation](https://docs.anthropic.com/en/docs/claude-code)
