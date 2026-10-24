# Echo Atlas — Verification Snapshot

**Project:** Godot game / Android deployment and validation project  
**Primary stack:** Godot 4.5.1, GDScript, Android export tooling, Git/GitHub  
**Source repository:** Private active-development repository

## Visual evidence

![Echo Atlas rendered verification captures](../assets/evidence/echo-atlas-verification.jpg)

*Rendered verification captures from the v0.2.0 automated UI journey: an opening sequence and a boss encounter. These are automated-review captures from the tested build, not claims of physical Android-device testing or human playtesting.*

## Verification record

A retained v0.2.0 verification report dated **3 October 2026** records a tested candidate with the following results:

| Check | Recorded result |
| --- | --- |
| Godot import | Passed with no script/parse/resource errors |
| Core suite | 8,342 assertions across 6 scenario groups; 0 failures |
| Boss simulations | 60/60 prepared level-five parties won; mean 24.5 rounds |
| Rendered UI journey | 334 assertions; full chapter, ending, recovery and title/continue; `failed=false` |
| Save isolation | Production save hashes unchanged during isolated testing |
| Older-save compatibility fixture | Passed load/re-save checks |
| Integrated art review | No blocking clipping/control-overlap/atlas/route-occlusion issue reported in reviewed captures |
| Signed Android APK | 74,545,861 bytes; APK signature schemes v2/v3 verified |
| Version continuity | Same package/signer; versionCode increased 1 → 2 |
| Android manifest | min API 24, target API 35; arm64-v8a and x86_64 |
| Exported-resource startup | Passed in the retained Linux/Godot validation environment |

The report explicitly notes that the 8,342 assertions include repeated combat-state invariants and are **not 8,342 independent test cases**.

## What the tests cover

The retained report describes coverage across:

- battle legality and state transitions,
- damage and replacement behavior,
- transactional saves and backup recovery,
- atlas metadata and malformed fallbacks,
- interaction routes and chapter progression,
- quests/forms/rewards,
- rendered UI flow,
- older save-schema compatibility,
- Android export/signature/manifest validation.

## Release evidence

The retained verification report records a signed v0.2.0 APK and keeps raw evidence in the private repository, including import/export logs, manifest checks, signature checks, update-continuity metadata, test logs and runtime captures.

## Explicit limitations

The verification report also records what was **not** proven for that candidate:

- no physical Android device/emulator runtime claim,
- no in-place phone installation claim,
- no claim that accelerated automation measures human enjoyment or natural pacing,
- no claim that the project had reached final visual quality.

Keeping these limitations in the evidence is intentional: the goal is credible engineering proof, not inflated claims.

This page is a sanitized public summary of the private repository's retained v0.2.0 verification material.
