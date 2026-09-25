# Decisions

- 2026-09-10: Start with a single-board 3v3 game; consider a three-board 3v3 relay match later.
- 2026-09-24: Use a fixed cycle for gameplay: teammates move in a set repeating order throughout the game.
- 2026-09-24: Earlier clock and single-board choices were exploratory. Superseded by the asynchronous three-board match decision below.
- 2026-09-24: Make the initial match three parallel chess games with three players per team. Each player can make their scheduled move on each board as turns become available; notifications alert them when a move is ready. Teams win the match by taking at least two boards. Use long per-move windows rather than short clocks.
- 2026-09-24: On each board, a team completes all three player moves in rotation before the opposing team can play its three moves. A player may advance to the next board only after both teammates have moved on the current board.
- 2026-09-24: A player may view and move only on the board currently assigned to them. After making their move, they cannot view that board again until their rotation returns, limiting board-based signaling between teammates.
- 2026-09-24: Replace the sequential per-board team move sequence with simultaneous assignments: each teammate moves on a different active board during the same team turn, then the opposing team moves. Rotate player-to-board assignments between turns so each player cycles through all active boards.
- 2026-09-24: Each team has a shared 24-hour active-time budget for a complete rotation, covering one move by each player on each of the three boards. The clock runs during that team turn, pauses during the opposing team turns, and resets when its rotation is complete. Timeout consequences remain undecided.
- 2026-09-24: When a board ends, continue the remaining boards and rotate any resulting bye fairly among teammates.
- 2026-09-24: Pivot from long asynchronous play and the 24-hour active-time rotation budget to timed, synchronous play. Clock durations and timeout thresholds remain open.
- 2026-09-24: When a player times out or bows out, remove them and open their seat for a replacement. Their team may wait for a replacement or forfeit the affected board and continue on the other two boards with two players. If no replacement joins before a further timeout, forfeit that board and continue on the remaining boards.
- 2026-09-24: The match winner is the team that wins at least two of the three boards.
