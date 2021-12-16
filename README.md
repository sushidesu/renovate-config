# sushidesu/renovate-config

## Usage

Add `github>sushidesu/renovate-config` to the "extends" array in your `renovate.json` file. It is not necessary to install any packages.

```json
{
  "extends": [
    "github>sushidesu/renovate-config",
    "some-other-config-you-use"
  ],
  "some-config": {
    // you can override config
  }
}
```

NOTE: This configuration includes `config: base`. Therefore, it is not necessary to include `config: base` in your `extends`.

## Settings Included


- Set timezone to `Asia/Tokyo`
- Open PR on every monday
- Add label `renovate`
- Grouping
  - patch (merge automatically)
  - minor
  - `@types/**`
  - linter,formatter (eg. eslint, prettier)
  - test packages (eg. jest, ts-jest, enzyme)

See [./default.json](./default.json) for more information.
