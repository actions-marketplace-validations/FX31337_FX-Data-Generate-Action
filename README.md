<!-- markdownlint-configure-file { "MD013": { "line_length": 120 } } -->
<!-- [![Release][github-release-image]][github-release-link] -->
<!-- [![Docker image][docker-build-image]][docker-build-link] -->
[![Status][gha-image-action-master]][gha-link-action-master]
[![Status][gha-image-docker-master]][gha-link-docker-master]
[![Status][gha-image-lint-master]][gha-link-lint-master]
[![][tg-channel-image]][tg-channel-link]
[![][tg-chat-image]][tg-chat-link]
[![Edit][gitpod-image]][gitpod-link]

# FX Data Generate 🐳 Action

This GitHub Action generates Forex historical data in CSV format.

## Supported formats

Supported formats:

- CSV

To convert CSV file into different formats, use [FX-Data-Convert-Action](https://github.com/EA31337/FX-Data-Convert-Action) action.

## File Inputs

### `OutputFile`

The CSV filename to generate data to. Default: `data`.

## Date Inputs

### `StartDate`

Starting date (in yyyy.mm.dd format). Default: `2020.01.01`.

### `EndDate`

Ending date (in yyyy.mm.dd format). Default: `2020.01.31`.

## Price Inputs

### `StartPrice`

Starting bid price. Default: `1.00`.

### `EndPrice`

Ending bid price. Default: `2.00`.

### `Digits`

Decimal digits of prices. Default: `5`.

### `Spread`

Spread between prices (in points).

## Modeling Inputs

### `Density`

Data points per minute.

### `Pattern`

Modeling patern to use. Default: `none`.

Supported patterns:

- `none`
- `curve`
- `random`
- `wave`
- `zigzag`

<!--
## Outputs

### `foo`

Foo bar.
-->

## Example usage

```yaml
uses: ea31337/fx-data-generate-action@master
```

### Support

- For bugs/features, raise a [new issue at GitHub](https://github.com/EA31337/FX-Data-Generate-Action/issues).
- Join our [Telegram group](https://t.me/EA31337) and [channel](https://t.me/EA31337_Announcements) for help.

<!-- Named links -->

[github-release-image]: https://img.shields.io/github/release/EA31337/FX-Data-Generate-Action.svg?logo=github
[github-release-link]: https://github.com/EA31337/FX-Data-Generate-Action/releases
<!-- Telegram links -->
[tg-channel-image]: https://img.shields.io/badge/Telegram-news-0088CC.svg?logo=telegram
[tg-channel-link]: https://t.me/EA31337_News
[tg-chat-image]: https://img.shields.io/badge/Telegram-chat-0088CC.svg?logo=telegram
[tg-chat-link]: https://t.me/EA31337
<!-- GitHub Actions build links -->
[gha-link-action-master]: https://github.com/EA31337/FX-Data-Generate-Action/actions?query=workflow%3AAction+branch%3Amaster
[gha-image-action-master]: https://github.com/EA31337/FX-Data-Generate-Action/workflows/Action/badge.svg
[gha-link-docker-master]: https://github.com/EA31337/FX-Data-Generate-Action/actions?query=workflow%3ADocker+branch%3Amaster
[gha-image-docker-master]: https://github.com/EA31337/FX-Data-Generate-Action/workflows/Docker/badge.svg
[gha-link-lint-master]: https://github.com/EA31337/FX-Data-Generate-Action/actions?query=workflow%3ALint+branch%3Amaster
[gha-image-lint-master]: https://github.com/EA31337/FX-Data-Generate-Action/workflows/Lint/badge.svg
<!-- Gitpod links -->
[gitpod-image]: https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod
[gitpod-link]: https://gitpod.io/#https://github.com/EA31337/FX-Data-Generate-Action