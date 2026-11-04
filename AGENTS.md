# AGENTS.md

Conventions for this repo. Follow them without being asked.

## Code ordering

**Do** order shell functions caller above callee, with `main` first.

## Writing

This applies to docs, comments, commit messages and anything else written in English.

**Do** use only these punctuation marks: `,` `.` `!` `:`

**Do** use markdown for formatting.

**Don't** use dashes, semicolons, parentheses or question marks in a sentence. Split the sentence in
two, or use a comma.

```
Do:    Build metadata is stamped at link time, so nothing reads it at runtime.
Don't: Build metadata is stamped at link time (via ldflags) — nothing reads it at runtime.
```

**Do** keep identifiers and tool names as they are spelled. `golangci-lint`, `homebrew-tap` and
`go-version-file` are names, not hyphenated prose.

## Commits

**Do** write semantic commit messages. Start with a type, then a colon, then what changed. Types:
`feat`, `fix`, `chore`, `test`, `docs`, `refactor`, `perf`, `build`, `ci`.

**Do** keep a commit message to one line.

**Don't** add a body, a bullet list, or a trailing attribution block.

```
Do:    feat: add version subcommand
Do:    fix: print command output to stdout instead of stderr
Do:    ci: pin golangci-lint installer by checksum
Don't: Added a version command

       - reports commit and build date
       - covered by a table test
```
