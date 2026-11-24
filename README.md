# Detached mirror of [bramstroker/homeassistant-powercalc](https://github.com/bramstroker/homeassistant-powercalc)

A backup that has **left the fork network**: it survives upstream being deleted, made private or taken down.

- Upstream branches and tags are under their normal names. This branch (`_mirror`) only holds the sync workflow.
- Rewritten or deleted upstream refs are kept under `_gone/<name>-<date>`. Nothing is ever dropped.
- Each run also fast-forwards [kvnloo/homeassistant-powercalc](https://github.com/kvnloo/homeassistant-powercalc) `master` (FF only, never force).
- Problems show up as issues labelled `mirror-alert`.

Sync logic: kvnloo/home tools/fork-standard (private). Git LFS objects aren't mirrored (pointer files only).
