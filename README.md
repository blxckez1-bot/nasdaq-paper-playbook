# Nasdaq Paper Playbook for Claude

A Claude skill for CME Micro E-mini Nasdaq-100 (MNQ) paper-trading research and setup review.

**[Download nasdaq-paper-playbook.zip](https://github.com/blxckez1-bot/nasdaq-paper-playbook/raw/refs/heads/main/nasdaq-paper-playbook.zip)**

## Install in Claude

1. Download the ZIP above.
2. Enable **Code execution and file creation** if needed.
3. Open **Customize > Skills > Create skill > Upload a skill**, upload the ZIP and enable it. Menu wording may vary.
4. Ask: **Use nasdaq-paper-playbook to explain the strategy and identify missing evidence before reviewing an MNQ paper setup.**

Upload this ZIP directly. If Brave or another browser blocks the raw download, use GitHub's **Code > Download ZIP**, extract that repository archive, then select the inner `nasdaq-paper-playbook.zip` for Claude.

For Claude Code, extract the skill folder into `~/.claude/skills/` or your project's `.claude/skills/`, then invoke `/nasdaq-paper-playbook`.

Official guides: [Claude Skills](https://support.claude.com/en/articles/12512180-use-skills-in-claude) and [Claude Code skills](https://code.claude.com/docs/en/skills).

## Included

- Fixed sweep/reclaim/higher-low research rules.
- Causal data and chronological validation requirements.
- Offline risk and evidence checks.
- Separate, unvalidated AM/PM breakout/retest research specifications.

## Status

**UNVALIDATED RESEARCH.** No historical backtest, expected return, win rate or implemented signal engine is supplied. Software checks do not establish profitability. The long-only helper cannot approve the separate AM/PM research; no Asia execution method is included.

Installation supplies no market feed, desktop controller, broker connection, scheduler or automatic orders. Account identity is initially unconfigured. It transfers no account history or trading authorization.

The planning reference is one MNQ, one position and 0.10% of fresh equity including costs, with a minimum USD15 stress reserve. These assumptions do not guarantee a maximum loss. Timely quotes, reviewed historical validation and fresh account/setup evidence remain required. Live/funded trading and paid data purchases are not authorized by this package.

The offline helper requires Python3.9+ and IANA timezone data. It uses the standard library, refuses output overwrites and always reports `order_authorized: false`.

Private account information is excluded. The portable document's distinct hash and source context appear in its provenance file. No open-source license has been selected.

## Verified package

The uploaded ZIP was downloaded and matched against the reviewed local package: **43,090 bytes**, 15 skill files. SHA-256:

```text
6b35474a78c416bb4880b82a4bd4dfa86d024c0da325151db785f583cb006e4d
```

31 synthetic helper checks passed during packaging. These checks are software verification, not historical trading validation.
