# ColorsHD — Early Color-Learning App Archive

Historical educational application for introducing basic color names in English through large full-screen colors, spoken pronunciation, and accompanying audio.

The repository preserves Android release artifacts, Windows / Unity build artifacts, and design materials from the original project. It is **not a complete Unity source project in its current state**.

Historical Google Play package reference from the previous README:

```text
com.Cubicle.projectColors
```

The old store URL should be treated as archival unless the listing is independently confirmed to still exist.

## Product concept

ColorsHD was designed around a very low-interaction learning loop:

```text
full-screen color
      |
      +-- English color name
      +-- spoken pronunciation
      +-- accompanying sound / music
      |
      v
next color
```

The original product description focused on seven basic colors and passive repetition rather than menus, quizzes, or complex navigation.

## Repository contents

### Android artifacts

`android/` contains pre-release distribution files including:

```text
ColorsHD v0.99 pre release.apk
ColorsHD v0.99 pre release.aab
ColorsHD v0.99 pre release 1.aab
```

plus poster / design assets.

These are **binary release artifacts**, not Android source code.

### Unity / Windows artifacts

`unity/` contains a built Unity application, including files such as:

```text
projectColors.exe
UnityPlayer.dll
UnityCrashHandler64.exe
projectColors_Data/
MonoBleedingEdge/
```

This is a compiled Unity / Windows distribution rather than the normal editable Unity project structure (`Assets/`, `Packages/`, `ProjectSettings/`).

Therefore this repository cannot currently reproduce the app from source through Unity Editor.

## Reproducibility gap

A maintainable Unity repository would normally contain:

```text
Assets/
Packages/
ProjectSettings/
```

plus source scripts, scenes, audio references, and build settings.

Those project-source directories are not present in the audited root. The current repository should therefore be presented as an **archive of builds and design assets**, not as an actively buildable Unity codebase.

## Child-directed product boundary

The old README used marketing language such as “make your child a genius” and suggested simply giving the phone to the child while the app does the rest.

That language is not appropriate as a factual educational claim. Repetition of colors and spoken labels can support exposure / familiarity, but this repository does not provide evidence of developmental, cognitive, or educational outcomes.

For a modern child-oriented product, use measured language such as:

> A simple color-recognition and English-pronunciation activity for supervised early-learning use.

## Screen-time / supervision

A passive visual / audio app for young children should not imply that caregiver involvement is unnecessary.

A modern version should consider:

- short guided sessions;
- caregiver controls;
- clear audio start / stop;
- no unnecessary engagement loops;
- no dark patterns;
- no behavioral advertising;
- no collection of data that is not required for the learning experience.

## Privacy policy in the old README

The previous README embedded a long privacy policy dated:

```text
2021-01-09
```

and referenced third-party services including:

```text
Google Play Services
Unity
```

That historical text should **not** be treated as a current privacy policy for a republished app.

Privacy disclosures must match the actual current build, SDKs, analytics, ads, crash reporting, permissions, storage, and store requirements.

### Contradictory child-privacy wording

The old policy said both that the product was intended for children and that the service “does not address anyone under the age of 13.” Those positions are inconsistent for a child-learning app.

Any future release should use a child-privacy policy specifically reviewed for the intended audience and markets.

## Binary distribution safety

Before redistributing the historical APK / AAB / EXE files:

- verify package identity;
- inspect requested permissions;
- verify signing certificates where relevant;
- scan historical binaries;
- confirm SDK / Unity version support;
- check whether embedded services or URLs are obsolete;
- document the exact build provenance.

Old binaries may no longer satisfy current Android / Google Play requirements.

## Repository size / source-control hygiene

The repository includes large compiled binaries such as Unity runtime DLLs and Android bundles.

For a modern engineering repository, prefer:

```text
source code in Git
      +
release binaries in GitHub Releases / artifact storage
```

rather than tracking large generated build outputs directly in the main source tree.

## Relationship to later learning experiments

The later `colorjoy-learn` repository explores a similar color-learning idea in a browser-based React implementation with timed color changes, ambient audio, and TTS experimentation.

For portfolio use, these can be presented as product evolution:

```text
ColorsHD
  -> early Unity / Android packaged learning app
  -> later ColorJoy browser / TTS experiment
```

rather than unrelated projects.

## Current status

**Historical educational-app distribution archive.** Android and Unity / Windows builds plus design assets are preserved, but the editable Unity source project is not present in the current repository.

## License

No repository-wide software / media license is assumed by this README. Verify rights separately for source material, audio, voice recordings, Unity assets, fonts, images, and compiled third-party components before redistribution.