# renovate-config

Shared [Renovate](https://docs.renovatebot.com/) preset for KloudLabs
repositories.

## Usage

Extend it from a repository's `renovate.json`:

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["github>kloudlabs-io/renovate-config"]
}
```

## What belongs here

Only policy shared by every repository: base presets, labels, vulnerability
alerts, lock file maintenance and the automerge rule for dev-only minor and
patch updates.

Rules specific to one repository, such as base branches, grouping or version
pins that must stay in step with another repo, stay in that repository.

## This repository is public

Public repositories extend this preset, so it is public too. Never add
credentials, `hostRules` with tokens or private registry details here.

## Validating

```shell
npx --yes --package renovate -- renovate-config-validator default.json
```
