# Install clip

About 45 seconds. One terminal, one empty folder, and the README. Node.js 22.20 or later. Make the type large enough to read. Do not show mail, tokens, or another project.

## What to type

From the empty folder:

```bash
npx --yes skills add frzxw/humanize --skill humanize -a cursor -y
```

One agent keeps the clip short. The README command names Claude Code, Cursor, and Codex when you want all three. `--yes` tells npx to install the `skills` package without asking. `-y` skips the questions from that CLI. If another prompt still appears, stop and retake.

## Order of shots

1. The README, held on Before and after. Show the long paragraph, then the two sentences under it. About 8 seconds.
2. The terminal in the empty folder. Type the command and let it finish. About 25 seconds.
3. The installed file. Run `ls .agents/skills/humanize` and open `SKILL.md` far enough to see `name: humanize`. About 10 seconds.

Stop on the file. The skill runs inside the agent after that. A chat reply will not fit in the minute.
