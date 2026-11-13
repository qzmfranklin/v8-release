# v8-release

First-party librusty_v8 static-library release assets for the `v8` Bazel
module of the gono monorepo.

The artifacts are built by `modules/v8/scripts/build-v8-staticlib.sh` under
the repo root's rules_clang toolchain + sysroots (plan
modules/v8/plan/0002-v8-rebootstrap.md), and published by
`modules/v8/scripts/publish-staticlibs.sh`.

Tag scheme: `v<crate-version>-firstparty[N]` -- one release per cut of the
five-triple set (linux amd64/arm64, windows amd64, darwin amd64/arm64).
Asset names are the v8 crate's own pin-table names, kept verbatim.
