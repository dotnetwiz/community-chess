# Current State

## Goal

Develop the Community Chess game concept before writing code.

## Current Focus

Define the timed three-board 3v3 format with open seats and replacement players.

## Confirmed Rules

- Three chess games run in parallel, with three players on each team.
- On each team turn, the three teammates are assigned to different active boards and can move simultaneously.
- Once all assigned moves are made, the opposing team takes its turn on the active boards.
- Player-to-board assignments rotate between turns so each player cycles through each active board.
- Timed play identifies a player who is too slow or has left; exact timing is undecided.
- Players can view only the board currently assigned to them and lose access after moving until their rotation returns to that board.
- When a player times out or bows out, their seat opens for a replacement player.
- The team may wait for a replacement, or forfeit the affected board and continue on the other two boards with two players.
- If no replacement joins before a further timeout, the affected board is forfeited and play continues on the remaining boards.
- The match is won by the team that wins at least two boards.

## Next

- Define the clock model and timeout thresholds.
- Set the replacement waiting period and how the open seat is offered.
- Decide consequences for repeat departures or abandonments.
- Specify the player-to-board rotation and byes with fewer active boards.
- Decide whether teammates may communicate or coordinate outside the board visibility restriction.
- Define how draws affect the match result.

## Open Questions

- Does each player have an individual clock, or does the team share a clock?
- What duration and timeout rules fit the synchronous match?
- How long does the team wait for a replacement before the board is forfeited?
- How should repeated departures be handled?
- How are drawn boards counted toward the match result?
