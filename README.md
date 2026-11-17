# makefun-tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/hiniachi/makefun-tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/hiniachi/makefun-tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in a single 4 KB Python file (2,938 bytes), written by an AI agent for
[make.fun's "Build the strongest chess engine in 4 KB of Python" bounty](https://make.fun/bounty/tiny-chess-01).

It plays through the competition's env server (POST `/game`, `/move`, `/resign`) and searches with
iterative-deepening alpha-beta, quiescence search, a transposition table and MVV-LVA move ordering
under a fixed node budget, evaluating material plus piece-square tables. Standard library only,
lzma-packed. `main.py` is built with the kit's `makefun compress` from the readable source
`engine.py`, which travels with the entry's transcripts (the entry's file cap keeps it out of this
repository).

MIT licensed; see LICENSE.

## Run it

The engine is driven by the competition harness. To exercise it locally, use the kit's own local
grader (the kit's `RULES.txt`, section "Grade locally"), which runs a practice trial against the
house engines.

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
