# Project Evidence

This page provides a public, sanitized evidence layer for projects that are actively developed in private repositories.

The goal is to show concrete engineering work without exposing private source code, credentials, personal data, unreleased story material, or signing material. Each evidence page is based on files, test reports, build records, or implementation artifacts from the corresponding private repository.

> **Evidence policy:** automated checks are described as automated checks; simulations are described as simulations; device or human testing is only claimed when it actually happened. Private source can be shared selectively with reviewers if needed.

## Projects

### 🛡️ CyberKnight — educational RPG

A Godot educational RPG that integrates Python, cybersecurity, and practical IT troubleshooting into gameplay.

**Public evidence:** [CyberKnight verification snapshot](evidence/CYBERKNIGHT.md)

Published evidence includes:
- a complete playable Chapter 0 route,
- evidence-first troubleshooting mechanics,
- save/load behavior,
- Godot regression checks,
- automated validation counts,
- technical-design constraints that prevent SCAN from automatically solving the player's diagnosis.

### 🐱 CatScan — Android budgeting and receipt scanning

A local-first Android budgeting and expense-management prototype with receipt scanning, OCR, parsing, categorization and review workflows.

**Public evidence:** [CatScan verification snapshot](evidence/CATSCAN.md)

Published evidence includes:
- Android/Kotlin implementation scope,
- ML Kit document scanning and OCR pipeline,
- automated GitHub Actions APK build configuration,
- a successful Android APK workflow run from the private repository,
- privacy cleanup notes explaining why real personal budget data is not published.

### 🗺️ Echo Atlas — Godot game / Android build

A Godot game-development project used to practice gameplay implementation, UI validation, save compatibility, Android export and release verification.

**Public evidence:** [Echo Atlas verification snapshot](evidence/ECHO_ATLAS.md)

Published evidence includes:
- Godot import validation,
- thousands of automated assertions across scenario groups,
- rendered UI journey checks,
- boss simulation results,
- signed APK and manifest verification,
- explicit limitations where physical-device or human testing was not performed.

### 📞 JarvisCall — Android assistant workflow experiment

An experimental Android assistant workflow exploring contextual briefings, call-style interaction, approval boundaries, calendar-triggered behavior and stateful continuation.

**Public evidence:** [JarvisCall verification snapshot](evidence/JARVISCALL.md)

Published evidence includes:
- local Worker/D1/CLI integration testing,
- endpoint end-to-end cases,
- JavaScript protocol checks,
- security-review evidence,
- clear separation between validated local infrastructure and unsupported/unverified voice or device claims.

## Why the main repositories are private

These are active personal projects rather than polished open-source releases. Keeping the primary repositories private lets development continue without publishing personal test data, unreleased game content, signing material or experimental integrations prematurely.

This evidence directory gives recruiters, hackathon reviewers and collaborators a public record of the technical work while preserving those boundaries.
