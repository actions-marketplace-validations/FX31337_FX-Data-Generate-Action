# FX Data Generate 🐳 Action

[![Tag][github-tag-image]][github-tag-link]
[![Status][gha-image-action-master]][gha-link-action-master]
[![Status][gha-image-docker-master]][gha-link-docker-master]
[![Status][gha-image-lint-master]][gha-link-lint-master]
[![Channel][tg-channel-image]][tg-channel-link]
[![Edit][gitpod-image]][gitpod-link]

This GitHub Action generates dummy Forex historical data in CSV format.

By default it generates the file in CSV format.

To convert CSV file to different formats,
use [FX-Data-Convert-Action](https://github.com/FX31337/FX-Data-Convert-Action) action.

## Usage

For full documentation, please read: [GitHub Actions Documentation](https://help.github.com/en/actions).

### Latest release

```yaml
uses: fx31337/fx-data-generate-action@v1
```

### Specific release

```yaml
uses: fx31337/fx-data-generate-action@v1.0.0
```

Note: Check _Releases_ for more details.

### Latest development version

```yaml
uses: fx31337/fx-data-generate-action@master
```

### Overriding default inputs

```yaml
uses: fx31337/fx-data-generate-action@master
with:
    Pattern: 'zigzag'
```

## Inputs

### File Inputs

#### `OutputFile`

The CSV filename to generate data to. Default: `data.csv`.

### Date Inputs

#### `StartDate`

Starting date (in yyyy.mm.dd format). Default: `2020.01.01`.

#### `EndDate`

Ending date (in yyyy.mm.dd format). Default: `2020.01.31`.

### Price Inputs

#### `StartPrice`

Starting bid price. Default: `1.00`.

#### `EndPrice`

Ending bid price. Default: `2.00`.

#### `Digits`

Decimal digits of prices. Default: `5`.

#### `Spread`

Spread between prices (in points).

### Modeling Inputs

#### `Density`

Data points per minute.

#### `Pattern`

Modeling pattern to use. Default: `none`.

Supported patterns:

- `none`
- `curve`
- `random`
- `wave`
- `zigzag`

#### `Volatility`

Volatility factor. Default: `1.0`.

### Other Inputs

#### `CmdArgs`

Extra arguments to pass to the script. Default: `-v` (for verbose output).

<!--
## Outputs

### `foo`

Foo bar.
-->

## Related actions

- To convert CSV file into different formats,
  use [FX-Data-Convert-Action](https://github.com/FX31337/FX-Data-Convert-Action)
  action.
- To generate CSV file instead,
  use [FX-Data-Generate-Action](https://github.com/FX31337/FX-Data-Generate-Action)
  action.

## Support

- For bugs/features, raise a [new issue at GitHub](https://github.com/FX31337/FX-Data-Generate-Action/issues).

<!-- Named links -->

[github-tag-image]: https://img.shields.io/github/tag/FX31337/FX-Data-Generate-Action.svg?logo=github
[github-tag-link]: https://github.com/FX31337/FX-Data-Generate-Action/tags

[tg-channel-image]: https://img.shields.io/badge/Telegram-join-0088CC.svg?logo=telegram
[tg-channel-link]: https://t.me/EA31337

[gha-link-action-master]: https://github.com/FX31337/FX-Data-Generate-Action/actions?query=workflow%3AAction+branch%3Amaster
[gha-image-action-master]: https://github.com/FX31337/FX-Data-Generate-Action/workflows/Action/badge.svg
[gha-link-docker-master]: https://github.com/FX31337/FX-Data-Generate-Action/actions?query=workflow%3ADocker+branch%3Amaster
[gha-image-docker-master]: https://github.com/FX31337/FX-Data-Generate-Action/workflows/Docker/badge.svg
[gha-link-lint-master]: https://github.com/FX31337/FX-Data-Generate-Action/actions?query=workflow%3ALint+branch%3Amaster
[gha-image-lint-master]: https://github.com/FX31337/FX-Data-Generate-Action/workflows/Lint/badge.svg

[gitpod-image]: https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod
[gitpod-link]: https://gitpod.io/#https://github.com/FX31337/FX-Data-Generate-Action
