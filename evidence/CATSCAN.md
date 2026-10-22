# CatScan — Verification Snapshot

**Project:** Local-first Android budgeting and receipt-scanning prototype  
**Primary stack:** Kotlin, Android, Jetpack Compose, Google ML Kit, GitHub Actions  
**Source repository:** Private active-development repository

## Implemented scope

The current prototype includes:

- budget dashboard and structured budget data,
- manual expense entry,
- Google ML Kit Document Scanner integration,
- ML Kit text recognition/OCR,
- language identification and supported on-device translation to English,
- receipt parsing for merchant, amount and category,
- a review step before an extracted receipt becomes a saved expense,
- local Android persistence without a CatScan account or application server,
- GitHub Actions APK builds.

The private source includes Kotlin UI/application logic that carries parsed receipt fields such as merchant, amount and category into an explicit review/save flow rather than silently accepting OCR output.

## Build pipeline evidence

The repository contains a GitHub Actions workflow that:

1. checks out the source,
2. configures Temurin Java 17,
3. installs Android platform/build tools,
4. configures Gradle 9.6,
5. runs `:app:assembleDebug`,
6. uploads the resulting debug APK as a workflow artifact.

A successful private workflow run on **22 October 2026** built the Android APK from the active development work. The retained successful run ID is `39763721161`.

## Product-development evidence

CatScan is being tested against real receipt failure modes rather than only ideal OCR samples. Development work has specifically focused on problems such as:

- totals being detected incorrectly,
- line-item text being interpreted poorly,
- category assignment being wrong even when the receipt wording is clear,
- reducing how much manual correction a user must perform.

That feedback has driven changes to both scanning/parsing logic and the overall budgeting workflow.

## Privacy boundary

Real personal budget values and private financial data are deliberately **not published** in this evidence repository. The private project documentation was also sanitized so the public proof demonstrates the application without exposing personal finances.

## Current limitations

CatScan remains an active prototype. A successful debug APK build proves the project compiles and packages through the configured Android CI pipeline; it does not by itself prove perfect OCR accuracy or production-store readiness.

This page is a sanitized public record derived from the private Android project and its build pipeline.
