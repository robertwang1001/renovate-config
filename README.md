# Renovate Configurations

This repository holds shared Renovate configuration presets for all my projects. By centralizing these settings, I can ensure consistency and simplify the maintenance of my dependency update rules.

## Available Presets

### Default Preset

The default configuration is intended to be used by most projects.

### NPM Project

Used by NPM projects.

## How to Use

> Go to [Github APP Renovate](https://github.com/apps/renovate) and click **configure** to add your repositories to Renovate

To use these presets in projects, extend the desired preset(s) in the `renovate.json` file. For example:

* Default preset

```json
{
  "extends": [
    "github>robertwang1001/renovate-config"
  ]
}
```

* Specified preset

```json
{
  "extends": [
    "github>robertwang1001/renovate-config:npm"
  ]
}
```

You can also set renovate [base branches](https://docs.renovatebot.com/configuration-options/#basebranches). For example scan and update only the `dev` branch

```json
{
  "baseBranches": [
    "dev"
  ]
}
```

> More GitHub preset usage, refer to https://docs.renovatebot.com/config-presets/#github
