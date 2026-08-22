# Persian Shar Skills

Agent skill for **شعر فارسی**: help people understand popular Persian poems and verses.

When the skill is active, It explains wording, each bayt, imagery, and common readings — not a general-purpose explainer and not a translator.

## Install

### Copy local files (beginner users)

No  tools required to be installed. Copy the `skills/persian-shar` directory in this repo and tell your agent that save this skill somewhere. 

### With Node.js

Requires Node.js (for `npx`). Then install with the [skills CLI](https://github.com/vercel-labs/skills):

```bash
npx skills add AmirHossein-z/persian-shar-skills
```

Examples:

```bash
# This repo, all skills
npx skills add AmirHossein-z/persian-shar-skills

# Only this skill
npx skills add AmirHossein-z/persian-shar-skills --skill persian-shar

# Global (all projects)
npx skills add AmirHossein-z/persian-shar-skills -g

# Specific well-known agents
npx skills add AmirHossein-z/persian-shar-skills -a cursor
npx skills add AmirHossein-z/persian-shar-skills -a claude-code
npx skills add AmirHossein-z/persian-shar-skills -a codex
npx skills add AmirHossein-z/persian-shar-skills -a github-copilot
npx skills add AmirHossein-z/persian-shar-skills -a antigravity
...

# Several agents at once
npx skills add AmirHossein-z/persian-shar-skills -a cursor -a claude-code -a codex
```

From a local clone:

```bash
npx skills add ./persian-shar-skills
```

After install, compatible agents (Cursor, Claude Code, Codex, and others supported by the CLI) pick up `SKILL.md` from the skill directory.

## Usage

Ask about a poem or a line, for example:

- این بیت حافظ یعنی چه؟ «اگر آن ترک شیرازی…»
- رباعی خیام را ساده توضیح بده
- این غزل مولانا دربارهٔ چیست؟
- تفاوت خوانش عرفانی و عاشقانهٔ این شعر چیست؟

## Repository structure

```
skills.sh.json                 # skills.sh repo page grouping
skills/persian-shar/
  SKILL.md                     # required skill metadata + instructions
  references/persian-poetry.md # poets, devices, sample walkthrough
```

## License

MIT license
