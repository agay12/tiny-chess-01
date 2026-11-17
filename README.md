# tiny-chess-01

A 3,894-byte chess engine entry for the make.fun tiny-chess-01 competition.

`main.py` is the whole engine: a 10x12 mailbox alpha-beta search with
iterative deepening, transposition table, killer moves, quiescence and an
incremental material + piece-square evaluation, under a fixed 60,000-node
budget per move (deterministic: no wall-clock decisions). It ships as an
lzma-compressed payload with its unpacker and speaks the competition's HTTP
env protocol.

Python 3.13, standard library only. MIT licensed; original code.
