# Custom Skills

Skills are folders of instructions, references, and resources that an agent loads when a task calls for them. They teach an agent to do a specific job the same way every time, so you stop repeating the same corrections in every prompt.

These skills follow the open [Agent Skills](https://agentskills.io) format, so they work with any agent that supports it rather than one product.

## About this repository

Every skill here began as feedback repeated often enough to be worth writing down once.

Each skill lives in its own folder under [`skills/`](./skills), self-contained, with a `SKILL.md` file holding its metadata and instructions. Longer material sits in separate files that the agent reads only when it needs them, which keeps the instructions short and the context small.

## Available skills

### [`technical-writing`](./skills/technical-writing)

Writes and edits documentation, slide copy, PDF content, README files, papers, and UI copy. It composes three modular skills, consulted in order, then adds an editing workflow and format-specific notes that tie them together.

Together they produce prose that reads clearly without simplifying the content. Complex material stays complex. What goes is the writing that obscured it.

### [`orwell-writing-rules`](./skills/orwell-writing-rules)

George Orwell's six rules from "Politics and the English Language" govern word and phrase choices: cut what you can, choose the short word, prefer the active, and break any rule rather than write something barbarous.

### [`google-style-guide`](./skills/google-style-guide)

Google's developer documentation style guide, adapted for scientific communication, sets voice and conventions: second person, active voice, sentence case, and no filler. The adaptation keeps precise technical terms that a plainer word would blur.

### [`scientific-writing-structure`](./skills/scientific-writing-structure)

Gopen and Swan's "The Science of Scientific Writing" supplies the structure that readers expect: subjects beside their verbs, old information opening a sentence, and the new, emphasized information at its end.

## Use a skill

Copy the skill folder into a directory your agent reads. Common locations:

| Agent | Personal skills | Project skills |
|---|---|---|
| Cursor | `~/.cursor/skills/` | `.cursor/skills/` |
| Claude Code | `~/.claude/skills/` | `.claude/skills/` |

For example, to install the technical-writing skill and the three skills it composes for Cursor:

```bash
git clone https://github.com/aadish98/custom-skills.git
mkdir -p ~/.cursor/skills
cp -r custom-skills/skills/technical-writing ~/.cursor/skills/
cp -r custom-skills/skills/orwell-writing-rules ~/.cursor/skills/
cp -r custom-skills/skills/google-style-guide ~/.cursor/skills/
cp -r custom-skills/skills/scientific-writing-structure ~/.cursor/skills/
```

Once installed, name the skill when you want it applied:

```text
Use the technical-writing skill to tighten the copy on these slides.
```

An agent can also load a skill unprompted when your request matches the skill's description. Ask one to draft release notes, and it should load the technical-writing skill without being told.

Check your agent's documentation for the directories it reads and any install command it provides.

## Repository structure

```text
custom-skills/
├── skills/
│   ├── technical-writing/
│   │   └── SKILL.md             # composes the three skills below
│   ├── orwell-writing-rules/
│   │   ├── SKILL.md             # metadata and instructions
│   │   └── reference.md         # detail, loaded on demand
│   ├── google-style-guide/
│   │   ├── SKILL.md
│   │   └── reference.md
│   └── scientific-writing-structure/
│       ├── SKILL.md
│       └── reference.md
├── LICENSE
└── README.md
```

## Create a skill

A skill is a folder with a `SKILL.md` file inside it:

```markdown
---
name: my-skill-name
description: Describes what the skill does and when an agent should use it.
---

# My skill

Add the instructions the agent should follow.
```

The frontmatter needs two fields:

- `name` — lowercase letters, numbers, and hyphens, matching the folder name.
- `description` — what the skill does and when to use it. An agent reads this to decide whether to load the skill, so name the tasks and terms that should trigger it. "Helps with documents" gives it nothing to match; "Extracts text and tables from PDF files. Use when the user mentions PDFs or forms" does.

Keep `SKILL.md` under 500 lines and move the details into files you link from it. For the full format, including the optional `license` and `compatibility` fields, see the [Agent Skills specification](https://agentskills.io/specification).

## Disclaimer

Test any skill in your own environment before you rely on it for work that matters. Behavior varies with the agent, the model, the tools available, and whatever else sits in the context window.

## License

Released under the [MIT License](./LICENSE).
