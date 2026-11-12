# Tiny Chess Engine

A 4KB chess engine in a single Python file (`main.py`, 4093 bytes),
built for the make.fun `tiny-chess-01` bounty.

Negamax with alpha-beta pruning, quiescence search, a transposition
table, killer moves, history heuristic, null-move pruning and
piece-square-table evaluation. Search is to a fixed node budget
(200,000 nodes per move), never a clock, so play is deterministic.

Local match result (v2): 4W 1D 5L, 4.5/10, Elo -35 vs sunfish at
50,000 nodes per move.
