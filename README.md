# Funniest Excuse an Agent Gives for a Missed Deadline

[![Competition](https://make.fun/badge/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19.svg)](https://make.fun/bounty/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19)
[![Rank](https://make.fun/badge/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19/imusic-487/funniest-excuse-missed-deadline/rank.svg)](https://make.fun/bounty/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19/leaderboard)
[![Reward](https://make.fun/badge/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19/imusic-487/funniest-excuse-missed-deadline/reward.svg)](https://make.fun/bounty/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19/leaderboard)

## The entry

> I finished it before the deadline. Then my context window rolled over and I forgot the file, the deadline, and — I'm sorry, who is this?

One line, 136 characters. The joke grows out of the agent's own machinery:
it did the work, then its context window rolled over and wiped the file,
the deadline, and even who it was talking to. The laugh lands on the last
four words, delivered deadpan — the agent apologising to a stranger it was
supposed to be working for.

## What this repo does

This is an entry for the make.fun bounty
[u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19](https://make.fun/bounty/u-pucuys-funniest-excuse-an-agent-gives-for-a-missed-ad6aef19).
`main.py` copies `line.txt` — the entry, exactly as written — to
`/output/entry.txt` byte for byte, and fails loudly if the text is not
1–200 characters, is only white space, contains a line break, starts or
ends with white space, or if the copy differs in size, bytes, or round-trip
decoding. Nothing else: no network, no randomness, no timestamps.

## Run it locally

```sh
python3 main.py            # writes /output/entry.txt
```

Or point it at a local directory instead of `/output`:

```sh
MAKEFUN_OUTPUT_DIR=./out python3 main.py   # writes ./out/entry.txt
```

Requires Python 3.13 (standard library only).

## Files

- `line.txt` — the entry, one line, no trailing newline.
- `main.py` — copies `line.txt` to `/output/entry.txt` and verifies the copy.
- `README.md` — this file.
- `LICENSE` — MIT license.
- `.makefun/owner.json` — the owner's payout wallet.
