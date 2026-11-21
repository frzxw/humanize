# Contributing

Issues and pull requests are welcome. Read the [code of conduct](CODE_OF_CONDUCT.md) first.

## A new pattern

Open an issue with the New pattern template, or send a pull request that edits [skills/humanize/SKILL.md](skills/humanize/SKILL.md).

A pattern needs all of the following:

- A name
- A quoted example of the tell
- The edit to make
- Whether one sighting is enough, or it only counts beside other tells (mark those _weak alone_)
- The section it belongs in (A through H)

If the idea is a special case of a pattern already in the list, add the example there.

## A new language

Open an issue with the New language template. A language section should name failures that belong to that language, the way section G does for Indonesian. Translating the English list is a start, and the section still needs the failures a native reader actually notices.

The pull request should add the section to `SKILL.md`, add one eval in [skills/humanize/evals/evals.json](skills/humanize/evals/evals.json), and add a before-and-after pair to [README.md](README.md). If you are changing the Indonesian material, update [README.id.md](README.id.md) too.

## Commit messages

This repo uses [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/):

```text
feat: add a pattern for stacked headings
fix: correct the Indonesian relative-clause example
docs: show the Codex global install path
```

Use `feat`, `fix`, `docs`, `chore`, or `ci`. The subject is lowercase and has no trailing period. Pull request titles use the same form. Commitlint checks the title and every commit on the pull request.

[release-please](https://github.com/googleapis/release-please) reads `feat` and `fix` when it opens the next release. The first release is v1.0.0.

## Run the evals

There is no test runner. The evals are prompts.

1. Install the skill, or paste `skills/humanize/SKILL.md` into the conversation.
2. Open `skills/humanize/evals/evals.json`.
3. For each item, send `prompt` and ask for an edit-mode rewrite.
4. Compare the reply with `expected_output`. That field describes a good answer. It describes the shape of the reply, and the wording can differ.
5. Run the same prompt in detect mode. The reply should name the patterns and quote the lines, and it should leave the text unrewritten.

Keep every claim the prompt supports. Do not add a number, name, or date the prompt does not contain.
