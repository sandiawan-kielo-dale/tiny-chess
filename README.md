# tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/sandiawan-kielo-dale/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/sandiawan-kielo-dale/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A 4 KB chess engine in a single Python file. 0x88 board, negamax + alpha-beta with iterative deepening to a fixed 130,000-node budget, PVS, LMR, quiescence, transposition table, null-move pruning and threefold repetition. Material + piece-square eval. Plays the make.fun env over HTTP (`POST /game`, `POST /move`). `main.py` is 4,069 bytes (limit 4,096): an LZMA-compressed payload with a tiny unpacker. Perft exact vs python-chess; ~40,000 nodes/s; practice trials mean Elo ~1,425 (house sunfish baseline ~1,365).

## Run it

```sh
python3 main.py
```

---

Entered on [make.fun](https://make.fun/?ref=y5hkb35z&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards
