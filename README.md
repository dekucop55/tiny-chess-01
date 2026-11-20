# tiny-chess-4k-engine

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/ItzSudhan/tiny-chess-4k-engine/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/ItzSudhan/tiny-chess-4k-engine/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in under 4 KB of Python (an lzma-packed `main.py`): 10x12 mailbox board seen from the side to move, full legal moves (castling, en passant, promotion; checked by perft), PVS alpha-beta with iterative deepening, transposition table, null move, late-move reductions, futility pruning, check extension, history ordering and quiescence search. Its piece-square tables are rebuilt at every root move: tapered by phase, with passed pawns, open files and pieces drawn to the enemy king. A small table picks, per opponent, colour and opening, the playing style that won fastest against the kit's house engines. It searches a fixed node budget per move, never a clock, so replays match.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=1pww8frk&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
