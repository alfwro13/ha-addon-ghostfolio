# 2.239.0

## Ghostfolio 2.239.0 Release Notes

### Added

- Added a new static portfolio analysis rule based on the total investment volume: _Fees_ (Fee Ratio)
- Extended the content of the _Self-Hosting_ section on the Frequently Asked Questions (FAQ) page with information on derived currencies

### Changed

- Deprecated the existing static portfolio analysis rule: _Fees_ (Fee Ratio)
- Ignored nested ETFs when fetching top holdings for ETF and mutual fund assets from _Yahoo Finance_
- Improved the scraper configuration with more detailed error messages
- Improved the language localization for German (`de`)
- Upgraded `@simplewebauthn/browser` and `@simplewebauthn/server` from version `13.1.0` to `13.2.2`
- Upgraded `cheerio` from version `1.0.0` to `1.2.0`

### Fixed

- Fixed the investment value by including currency effects in the portfolio summary tab on the home page
- Added the missing `valueInBaseCurrency` to the response of the import activities endpoint

### Special Thanks

- @dtslvr
- @KenTandrian
- @veeceey

---
*This release was automatically generated based on the official Ghostfolio update.*

---

CHANGELOG.md
