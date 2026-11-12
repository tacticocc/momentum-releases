# Momentum release notes

This repository publishes public release notes for Momentum. Download and installer delivery lives on the [Momentum download page](https://momentumachines.com/download/).

## Publish notes

Create a GitHub Release with a tag that exactly matches the product version, such as `v1.2.3.4`. Use the GitHub Release body for the public notes and publish it as a normal release. Leave the asset list empty.

Use this structure for the release body:

```markdown
A short summary of what people will notice in this release.

## New

- A user-facing feature.

## Improved

- A change to an existing workflow.

## Fixed

- A problem this release resolves.
```

Use only the sections that apply. Keep the summary and first few bullets short enough for Discord. The announcement links back to the full notes.

Momentum Bot checks for the matching published notes and signed production update at `/v2/stable.json`. Either can be ready first. When both are available, it posts one announcement for the version in the Momentum Discord `#releases` channel. The post links to downloads and the GitHub Release.
