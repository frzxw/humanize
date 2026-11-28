# humanize

A skill that takes the AI tells out of prose.

The instructions live in [skills/humanize/SKILL.md](skills/humanize/SKILL.md): 38 patterns, a detect mode and an edit mode, and a short note on how to apply them in chat and in a repository.

## Before and after

This is a launch note with two facts in it: a billing page is live, and people can download the last 12 invoices as PDF. The second version is the same paragraph after edit mode in the skill. The facts stay. The announcement, the sales language, the contrast, and the closer go.

Before:

> We are thrilled to announce that the new billing page is live, marking a pivotal moment in our journey. Nestled in the heart of the product, this cutting-edge page uses a robust design to empower users, streamline invoice work, and unlock clarity. It is not just a page, it is a clearer way to see invoices. Users can download the last 12 invoices as PDF, highlighting our commitment to transparency. In today's world, that is the real win.

After:

> The new billing page is live. Users can download the last 12 invoices as PDF.

## Install

From the project you want the skill in, with Node.js 22.20 or later:

```bash
npx skills add frzxw/humanize
```

The CLI asks which agents to install into. To skip the questions:

```bash
npx skills add frzxw/humanize --skill humanize -a claude-code -a cursor -a codex -y
```

Add `-g` to install for every project on the machine.

## Install by hand

Copy the [skills/humanize](skills/humanize) folder to the path your agent reads.

| Agent | In one project | For every project |
| --- | --- | --- |
| Claude Code | `.claude/skills/humanize` | `~/.claude/skills/humanize` |
| Cursor | `.agents/skills/humanize` | `~/.cursor/skills/humanize` |
| Codex | `.agents/skills/humanize` | `~/.codex/skills/humanize` |

Cursor also reads `.cursor/skills/humanize` in a project. Codex also reads `~/.agents/skills/humanize`.

## What is different

The first 26 patterns come from [blader/humanizer](https://github.com/blader/humanizer) by Siqi Chen, which distills Wikipedia's [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing). Further patterns come from [petergyang/no-ai-slop](https://github.com/petergyang/no-ai-slop) by Peter Yang.

Four patterns are original here:

- 28, over-structuring
- 35, length that does not match the question
- 37, announcing the work instead of doing it
- 38, invented specifics

The skill also says how to use it in a chat reply and in repository text: lead with the decision, keep one topic per message, and keep commit and merge messages free of em dashes.

## Contributing

Pattern ideas, language additions, and bug reports go through [CONTRIBUTING.md](CONTRIBUTING.md). The code of conduct is [Contributor Covenant 2.1](CODE_OF_CONDUCT.md).

## Credits

- Siqi Chen, [blader/humanizer](https://github.com/blader/humanizer), MIT
- Peter Yang, [petergyang/no-ai-slop](https://github.com/petergyang/no-ai-slop), MIT
- Wikipedia contributors, [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing)

License texts for the two upstream projects are in [skills/humanize/licenses](skills/humanize/licenses). This repository is MIT. See [LICENSE](LICENSE) and [NOTICE](NOTICE). The same permission notice is in [skills/humanize/LICENSE](skills/humanize/LICENSE), so an install keeps it.

## Made by Fariz Wibisono

I write and build in public.

- Site: [frzxw.me](https://frzxw.me)
- X: [@frzwibisono](https://x.com/frzwibisono)
- LinkedIn: [frzxw](https://www.linkedin.com/in/frzxw)
- GitHub: [frzxw](https://github.com/frzxw)
