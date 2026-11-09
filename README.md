# Solvenger Employee — Android APK mirror

This repository contains no source code. Its releases carry the signed Solvenger Employee Android APK
as a download mirror for networks where the primary Solvenger download host is unreachable.

- Each release `employee-android-<versionName>-<versionCode>` has exactly one asset with the immutable name
  `solvenger-employee-<versionName>-<versionCode>-<sha256>.apk`, byte-identical to the APK published at
  `https://solvenger.app/downloads/employee/android/`.
- The Solvenger app verifies the SHA-256, size and signing certificate from the trusted
  `https://solvenger.app/downloads/employee/android/latest.json` manifest before installing.
- Signing certificate SHA-256: `2CD9A1EC28B223BCA07FB5EC2772FA2F41516EA5116487814892CB43B6476B30`.

Releases are published by `scripts/android/publish-github-mirror.sh` in the private Solvenger frontend repository.
