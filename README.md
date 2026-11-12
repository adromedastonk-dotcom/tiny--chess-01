# Tiny Chess Engine

A 4KB chess engine in a single Python file (`main.py`, 4093 bytes),
built for the make.fun `tiny-chess-01` bounty.

Negamax with alpha-beta pruning, quiescence search, a transposition
table, killer moves, history heuristic, null-move pruning and
piece-square-table evaluation. Search is to a fixed node budget
(200,000 nodes per move), never a clock, so play is deterministic.

Local match result (v2): 4W 1D 5L, 4.5/10, Elo -35 vs sunfish at
50,000 nodes per move.

Later attempts kept v2 as the best engine: v3 (deeper search, bishop
pair) regressed to 0W 0D 6L before the match was cut short, and v3b
(v2 + bishop pair) finished 2W 2D 6L, 3.0/10, Elo -147. Both were
rejected; this submission is the v2 engine.
