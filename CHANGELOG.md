# 2.242.0

## Ghostfolio 2.242.0 Release Notes

### Changed

- Changed the account field to optional in the create or update activity dialog

### Fixed

- Fixed a validation issue for valuables used in the create and import activity logic
- Fixed the page size for presets in the historical market data table of the admin control panel

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 2.241.0

## Ghostfolio 2.241.0 Release Notes

### Changed

- Improved the usability of the portfolio summary tab on the home page in the _Presenter View_
- Refreshed the cryptocurrencies list
- Improved the language localization for German (`de`)
- Improved the language localization for Spanish (`es`)

### Fixed

- Fixed an issue with `balanceInBaseCurrency` of the accounts in the value redaction interceptor for the impersonation mode
- Fixed an issue with `comment` of the accounts in the value redaction interceptor for the impersonation mode
- Fixed an issue with `dividendInBaseCurrency` of the accounts in the value redaction interceptor for the impersonation mode
- Fixed an issue with `interestInBaseCurrency` of the accounts in the value redaction interceptor for the impersonation mode
- Fixed an issue with `value` of the accounts in the value redaction interceptor for the impersonation mode

### Special Thanks

- @dtslvr
- @KenTandrian
- @slegarraga

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 2.240.0

## Ghostfolio 2.240.0 Release Notes

### Added

- Added a _No Activities_ preset to the historical market data table of the admin control panel
- Added support for custom cryptocurrencies defined in the database
- Added support for the cryptocurrency _Sky_

### Changed

- Harmonized the validation for the create activity endpoint with the existing import activity logic
- Upgraded `marked` from version `17.0.1` to `17.0.2`
- Upgraded `ngx-markdown` from version `21.0.1` to `21.1.0`

### Special Thanks

- @DavidReque
- @dtslvr
- @KenTandrian

---
*This release was automatically generated based on the official Ghostfolio update.*

---

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
