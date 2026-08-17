# Completion plan

1. Treat `master` as the historical base and document ColorsHD from the repository evidence: Android release packages/design assets plus a checked-in Unity runtime/build tree; do not present it as a modern source-first app until canonical source is verified.
2. Reconcile the 5.7 KB README with what can actually be reproduced, including the shipped `v0.99 pre release` APK/AAB artifacts, platform targets and whether original Unity project source/assets are complete.
3. Identify the canonical implementation and provenance of the `android` and `unity` directories; distinguish source, exported player/runtime files, release binaries and design/archive material.
4. Remove large APK/AAB/generated Unity runtime/build artifacts from normal Git history going forward (preserve releases separately if historically important) and add repository hygiene rules for generated binaries/caches.
5. Pin the historical Unity editor, Android Gradle/SDK/JDK and build settings only where they can be recovered from project metadata; otherwise document the exact reproducibility gap instead of guessing versions.
6. Audit obsolete Android/Unity APIs, permissions and third-party packages before any attempt to republish; do not ship the historical binary as current without a security/platform compatibility review.
7. Recover/test the core color/game logic from source if present and add deterministic smoke tests; if only compiled runtime remains, classify the project as archival rather than fabricating a maintainable test suite.
8. Restrict `.github` automation to reproducible checks such as repository hygiene/source validation, adding Android/Unity builds only after a clean source project builds locally in a pinned environment.
9. Curate the existing design screenshots/posters and historical release notes into a portfolio case study showing the product, original platform and era without implying current store availability.
10. Make an explicit final decision: modernize from recovered source in a clean repository, or preserve ColorsHD as an archival shipped-project case study; keep legacy binaries out of the active-development path.
