# tiny-chess-01 entry

A chess engine in one 4 KB Python file (lzma-packed, standard library only).
It talks to the make.fun env (POST /game, /move, /resign) and searches with
iterative deepening alpha-beta, quiescence, a transposition table and MVV-LVA
move ordering under a fixed node budget, evaluating material plus piece-square
tables. `main.py` is packed with the kit's `makefun compress` from the readable source
`engine.py`; the source is uploaded with the entry's transcripts (the entry's
file cap keeps it out of the repository).

MIT licensed; see LICENSE.
