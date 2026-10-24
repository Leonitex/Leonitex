# CyberKnight — Verification Snapshot

**Project:** Educational RPG / technical learning game  
**Primary stack:** Godot, GDScript, Python, Git/GitHub  
**Source repository:** Private active-development repository

## Visual evidence

![CyberKnight Chapter 0 bedroom scene](../assets/evidence/cyberknight-bedroom.jpg)

*Sanitized thumbnail of the illustrated bedroom scene asset used by the playable Chapter 0 vertical slice. It is shown as development evidence, not as a claim of final production art.*

## What exists

CyberKnight has a playable Chapter 0 route that begins with character setup, moves through an illustrated bedroom/work sequence, transitions into the alternate world, introduces the companion character, and ends with an evidence-first relay troubleshooting challenge and chapter-end save checkpoint.

The technical learning loop is intentionally designed so that **SCAN gathers evidence but does not diagnose the fault for the player**. The player must inspect components, compare observations, make a diagnosis, apply the correct configuration and confirm the repair.

## Automated verification snapshot

The private repository's Chapter 0 technical guide records the following regression results from the playable slice:

| Validation | Result |
| --- | ---: |
| Chapter 0 full-flow checks | 67 passed |
| A.5 bedroom checks | 108 passed |
| A.5 component checks | 71 passed |
| Milestone A checks | 96 passed |
| Bedroom/desktop round-trip | Passed |
| Godot headless import | Passed |
| Python tests | Passed |

The documented test environment used Godot 4.7.2 Compatibility renderer.

These numbers are automated checks, not claims of hundreds of independent human test cases.

## Example engineering behavior

A representative part of the private implementation tracks five pieces of relay evidence before the UI advances from investigation to diagnosis. The game separately tracks correct diagnosis, configuration and final repair state. This supports the educational rule:

> **Gather evidence → compare → diagnose → configure → confirm.**

The source also prevents interaction unless the player is physically near an authored interaction point and uses a walkability policy for reachability.

## Why this is useful evidence

This demonstrates more than a concept document. The project includes:

- working Godot scenes and player interaction,
- state/progression tracking,
- dialogue and chapter flow,
- save/load checkpoint behavior,
- evidence-gated troubleshooting mechanics,
- regression tests around existing gameplay systems,
- design documentation that constrains implementation behavior.

## Current limitations

The published snapshot does **not** claim final production art, final animation quality, a completed full game, or finished Chapter 1. Some Chapter 0 presentation assets are still prototype-quality and the project remains in active development.

This page is a sanitized public record derived from the private repository's playable-slice documentation and implementation evidence.
