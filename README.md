# Creator agent skills

Claude skills for running a YouTube channel, plus a `cross-check` skill that verifies answers from several angles before giving a final one. Free, MIT.

**These skills write. You upload.** Nothing is published for you.

## Skills

| command | what it does |
| --- | --- |
| `/yt-script` | Idea to spoken script, 5 scored hooks |
| `/yt-package` | Title + thumbnail checked as one pairing |
| `/yt-shorts` | Shorts found inside a long transcript |
| `/yt-plan` | A week that fits your real hours |
| `cross-check` | Fact-checker, skeptic, missing-piece and bias critics, then a final answer that follows evidence |

## Install (Claude Code)

```bash
git clone https://github.com/YOUR-USERNAME/creator-agent-skills.git
mkdir -p ~/.claude/skills
cp -r creator-agent-skills/skills/* ~/.claude/skills/
```

No Claude Code? Paste any single `SKILL.md` at the top of a chat and it runs as a mode.

## Voice file

Copy `templates/voice.md` to `~/.claude/youtube/voice.md` and fill it in (10 minutes). Or send Claude 3 of your transcripts and say "write my voice.md from these".

## Using cross-check with ChatGPT and Gemini

1. Ask the same question to Claude, ChatGPT and Gemini.
2. Paste each answer into the others: "Find mistakes, invented facts, missing points."
3. Paste everything into one chat: "Keep what all agree on, resolve disagreements by evidence, ignore what I would like to hear."

All models can share the same mistake, so check numbers and facts against a real source.

## Limits

- Hook scores are a rough checklist, not a predictor.
- Early version, not tested at scale. Issues and pull requests welcome.

## Licence

MIT.
