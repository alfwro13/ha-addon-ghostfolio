# 3.24.0

## Ghostfolio 3.24.0 Release Notes

### Added

- Exposed the `DATA_SOURCE_FEAR_AND_GREED_INDEX_STOCKS` environment variable to set the data source of the _Fear & Greed Index_ (market mood)
- Exposed the `ENABLE_FEATURE_RATE_LIMITING` environment variable to control rate limiting for authentication and sign-up endpoints
- Exposed the `TRUST_PROXY` environment variable to determine the client IP address when running behind a reverse proxy

### Changed

- Rounded the value of the _Fear & Greed Index_ (market mood)
- Improved the language localization for Korean (`ko`)

### Special Thanks

- @dtslvr
- @KenTandrian
- @moduvoice

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.23.0

## Ghostfolio 3.23.0 Release Notes

### Changed

- Migrated the deprecated `@nx/webpack:webpack` executor to `@nx/webpack/plugin`
- Set the change detection strategy to `OnPush` in the about page
- Set the change detection strategy to `OnPush` in the admin control panel
- Set the change detection strategy to `OnPush` in the blog page components
- Set the change detection strategy to `OnPush` in the Frequently Asked Questions (FAQ) page
- Set the change detection strategy to `OnPush` in the home page
- Set the change detection strategy to `OnPush` in the markets overview
- Set the change detection strategy to `OnPush` in the resources page
- Set the change detection strategy to `OnPush` in the user account page
- Set the change detection strategy to `OnPush` in the _Zen Mode_
- Improved the language localization for Chinese (`zh`)
- Improved the language localization for German (`de`)

### Special Thanks

- @Arjun8242
- @dtslvr
- @KenTandrian
- @qiukui666

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.22.0

## Ghostfolio 3.22.0 Release Notes

### Added

- Added support for a copy-to-clipboard action in the alert dialog component

### Changed

- Improved the user account deletion flow in the user settings of the user account page
- Improved the date formatting of the first activity in the historical market data table of the admin control panel
- Set the change detection strategy to `OnPush` in the activities page
- Set the change detection strategy to `OnPush` in the allocations page
- Set the change detection strategy to `OnPush` in the analysis page
- Set the change detection strategy to `OnPush` in the portfolio holdings page
- Set the change detection strategy to `OnPush` in the activities page
- Set the change detection strategy to `OnPush` in the _FIRE_ page
- Set the change detection strategy to `OnPush` in the users section of the admin control panel
- Hardened the endpoint to update a property of the admin control panel by validating the `key` path parameter
- Renamed the `SymbolProfileOverrides` _Prisma_ data model to `AssetProfileOverrides` while keeping the database table name
- Improved the language localization for Dutch (`nl`)
- Improved the language localization for French (`fr`)
- Improved the language localization for German (`de`)

### Special Thanks

- @Aftab3008
- @archit-goyal
- @Arjun8242
- @DavidReque
- @dtslvr
- @KenTandrian
- @munzzyy
- @SlavaDoroshenko
- @youdie006

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.21.0

## Ghostfolio 3.21.0 Release Notes

### Added

- Added support for tags in the account (experimental)
- Exposed the `PROCESSOR_PORTFOLIO_SNAPSHOT_COMPUTATION_REMOVE_ON_FAIL` environment variable to control the removal of failed jobs in the portfolio snapshot computation queue

### Changed

- Set the change detection strategy to `OnPush` in the alert dialog component
- Set the change detection strategy to `OnPush` in the confirmation dialog component
- Set the change detection strategy to `OnPush` in the prompt dialog component
- Set the change detection strategy to `OnPush` in the overview of the admin control panel
- Set the change detection strategy to `OnPush` in the portfolio page
- Deprecated the `isExcluded` attribute of the account in favor of the _Exclude from Analysis_ tag
- Improved the language localization in the users table of the admin control panel
- Improved the language localization for German (`de`)
- Upgraded `envalid` from version `8.1.1` to `8.2.0`
- Upgraded `stripe` from version `21.0.1` to `22.2.3`

### Fixed

- Fixed an issue with the custom tags of the user in the import functionality
- Fixed the creation of the _Stripe_ checkout session for languages not supported by _Stripe_ (`ca` and `uk`)
- Fixed the error handling in the endpoint to create a _Stripe_ checkout session

### Special Thanks

- @Aftab3008
- @AkashNegi1
- @DavidReque
- @dtslvr
- @ylink-lfs

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.20.0

## Ghostfolio 3.20.0 Release Notes

### Changed

- Refactored the rounding logic in the holding detail dialog
- Refactored the rounding logic in the treemap chart component
- Restricted the modification of activity tags in the impersonation mode
- Hardened the endpoint of the public access for portfolio sharing by restricting it to public accesses
- Improved the parsing of integer query parameters (`skip` and `take`) in the `GET api/v1/admin/user` endpoint
- Improved the parsing of integer query parameters (`skip` and `take`) in the `GET api/v1/asset-profiles` endpoint
- Improved the parsing of the integer query parameter (`includeHistoricalData`) in the `GET api/v1/market-data/markets` endpoint
- Improved the parsing of the integer query parameter (`includeHistoricalData`) in the `GET api/v1/symbol/:dataSource/:symbol` endpoint
- Harmonized the filter parsing using `groupBy` across various services
- Improved the language localization by translating various tooltips across the application
- Improved the language localization for German (`de`)
- Improved the language localization for Ukrainian (`uk`)
- Upgraded `yahoo-finance2` from version `3.14.3` to `3.15.4`

### Fixed

- Resolved an issue in the treemap chart component when the holdings list is empty
- Fixed the handling of cash positions in the portfolio calculations when filtering by holding or tag
- Fixed the handling of cash positions in the portfolio details when filtering
- Fixed the market condition of the benchmarks in the twitter bot service when values round to zero

### Special Thanks

- @Aftab3008
- @Arjun8242
- @dtslvr
- @KenTandrian

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.19.1

## Ghostfolio 3.19.1 Release Notes

### Added

- Added support for routing outgoing requests through a per-domain proxy via the `PROXY_ROUTES` setting in the `FetchService`
- Added `@prisma/config` as a development dependency used by the _Prisma Configuration File_

### Changed

- Harmonized the date picker styling across various components
- Updated the _Privacy Policy_
- Updated the _Terms of Service_
- Improved the parsing of integer query parameters (`skip` and `take`) in the `GET api/v1/activities` endpoint
- Improved the language localization for German (`de`)
- Improved the language localization for Japanese (`ja`)
- Upgraded `@ionic/angular` from version `8.8.5` to `8.8.12`
- Upgraded `nestjs` from version `11.1.21` to `11.1.27`

### Fixed

- Fixed an issue where values incorrectly rounded to negative zero in the value component
- Fixed the colorization of the change from all time high in the benchmark component when values round to zero
- Fixed the market condition of the benchmarks when values round to zero
- Fixed the validation of the data source field of an asset profile with market data
- Fixed a recurring issue where single-value fields were incorrectly validated as arrays in various endpoints

### Special Thanks

- @Aftab3008
- @AkashNegi1
- @dtslvr
- @KenTandrian
- @SeineEloquenz
- @slagiewka

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.19.0

## Ghostfolio 3.19.0 Release Notes

### Added

- Added support for routing outgoing requests through a per-domain proxy via the `PROXY_ROUTES` setting in the `FetchService`
- Added `@prisma/config` as a development dependency used by the _Prisma Configuration File_

### Changed

- Updated the _Privacy Policy_
- Updated the _Terms of Service_
- Improved the parsing of integer query parameters (`skip` and `take`) in the `GET api/v1/activities` endpoint
- Improved the language localization for German (`de`)
- Improved the language localization for Japanese (`ja`)
- Upgraded `@ionic/angular` from version `8.8.5` to `8.8.12`
- Upgraded `nestjs` from version `11.1.21` to `11.1.27`

### Fixed

- Fixed the validation of the data source field of an asset profile with market data
- Fixed a recurring issue where single-value fields were incorrectly validated as arrays in various endpoints

### Special Thanks

- @Aftab3008
- @AkashNegi1
- @dtslvr
- @KenTandrian
- @SeineEloquenz
- @slagiewka

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.18.0

## Ghostfolio 3.18.0 Release Notes

### Added

- Added support for filtering in the public access for portfolio sharing (experimental)
- Set up the language localization for Japanese (`ja`)

### Changed

- Improved the alias display in the access table to share the portfolio
- Improved the language localization for German (`de`)

### Fixed

- Fixed a phantom `UNKNOWN` slice in the portfolio proportion chart component caused by floating-point rounding
- Fixed the base currency for the total value calculation in the public access for portfolio sharing
- Fixed an issue in the public access for portfolio sharing that exposed absolute values of the top holdings of ETFs
- Fixed the time zone handling in the `api` test suite for deterministic execution in `UTC`

### Special Thanks

- @dtslvr
- @gmag11
- @greymoth-jp

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.17.0

## Ghostfolio 3.17.0 Release Notes

### Added

- Added `zod` as a root dependency to resolve peer dependency warnings

### Changed

- Improved the error message styling in the import activities dialog
- Improved the grantee display in the access table to share the portfolio
- Improved the country mapping for data providers
- Upgraded `bull-board` from version `7.2.1` to `8.0.1`
- Upgraded `Nx` from version `22.7.5` to `23.0.1`
- Upgraded `prettier` from version `3.8.3` to `3.8.4`

### Fixed

- Improved the table headers’ alignment in the queue jobs table of the admin control panel

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.16.0

## Ghostfolio 3.16.0 Release Notes

### Added

- Extended the user account settings with a copy-to-clipboard button for the user id
- Added pagination to the platform management of the admin control panel
- Added pagination to the tag management of the admin control panel
- Extended the asset profile details dialog of the admin control panel with a copy-to-clipboard button for the ISIN number
- Extended the asset profile details dialog of the admin control panel with a copy-to-clipboard button for the symbol

### Changed

- Improved the throughput of the market data gathering queue by applying the rate limit per data source
- Decreased the rate limiter duration of the market data gathering queue jobs from 4 to 3 seconds
- Removed the deprecated `SymbolProfile` field from the endpoint `GET api/v1/portfolio/holding/:dataSource/:symbol`
- Upgraded `@simplewebauthn/browser` and `@simplewebauthn/server` from version `13.2.2` to `13.3`

### Fixed

- Fixed an issue with hourly market data updates not refreshing prices for asset profiles with `MANUAL` data source
- Fixed an issue with the log context formatting in the performance logging service

### Special Thanks

- @AkashNegi1
- @dtslvr

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.15.1

## Ghostfolio 3.15.1 Release Notes

### Changed

- Improved the dynamic numerical precision for various values in the account detail dialog on mobile
- Improved the dynamic numerical precision for various values in the holding detail dialog on mobile
- Upgraded `@internationalized/number` from version `3.6.6` to `3.6.7`

### Fixed

- Fixed an issue where symbols with special characters caused API request failures by URL encoding the symbol
- Fixed the disabled state of the delete action in the asset profiles actions menu of the historical market data table in the admin control panel
- Fixed the persistence of an empty `locale` string in the scraper configuration
- Fixed a transaction timeout that prevented gathering historical market data for symbols with a long history
- Fixed an exception in various portfolio endpoints when historical exchange rate data is missing

### Special Thanks

- @dtslvr
- @KenTandrian

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.14.0

## Ghostfolio 3.14.0 Release Notes

### Added

- Exposed the `ENABLE_FEATURE_CRON` environment variable to control scheduled cron job execution
- Exposed the `PROCESSOR_GATHER_STATISTICS_CONCURRENCY` environment variable to control the concurrency of the statistics gathering queue processor

### Changed

- Consolidated the exchange rates to be gathered with hourly market data
- Improved the language localization for German (`de`)
- Upgraded `@openrouter/ai-sdk-provider` from version `2.9.0` to `2.9.1`
- Upgraded `undici` from version `7.24.4` to `8.5.0`

### Fixed

- Fixed an issue in the data provider service where asset profiles and historical data could be missing for symbols that exist in multiple data sources by keying the responses by the asset profile identifier
- Resolved an exception in the benchmarks service when the current market price is unavailable

### Special Thanks

- @dtslvr
- @KenTandrian

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.13.0

## Ghostfolio 3.13.0 Release Notes

### Added

- Added an icon to indicate external links in the page tabs component
- Added the Korean (`ko`) language to the footer
- Added a data gathering frequency (`DAILY` or `HOURLY`) to the asset profile to control the market data gathering interval

### Changed

- Changed the _Fear & Greed Index_ (market mood) in the markets overview to use the stored market data instead of a live quote
- Moved the endpoint to get the asset profiles from `GET api/v1/admin/market-data` to `GET api/v1/asset-profiles`
- Added the selected asset profile count to the delete menu item of the historical market data table in the admin control panel
- Added the selected asset profile count to the deletion confirmation dialog of the historical market data table in the admin control panel
- Improved the sorting to be case-insensitive in the platform management of the admin control panel
- Improved the sorting to be case-insensitive in the tag management of the admin control panel
- Improved the language localization for German (`de`)
- Upgraded `yahoo-finance2` from version `3.14.2` to `3.15.3`

### Fixed

- Fixed an issue with the localization of the country names
- Fixed an issue in the data provider service where quotes could be missing for symbols that exist in multiple data sources by keying the quotes response by the asset profile identifier

### Special Thanks

- @AkashNegi1
- @DavidReque
- @dtslvr
- @KenTandrian
- @Sjohn21

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.12.0

## Ghostfolio 3.12.0 Release Notes

### Changed

- Improved the styling of the checkboxes to consistently use the primary color in their states
- Improved the account name display in the accounts table
- Improved the name display in the activities table
- Improved the last activity display in the users table of the admin control panel
- Improved the registration display in the users table of the admin control panel
- Improved the user id display in the users table of the admin control panel
- Deprecated `SymbolProfile` in favor of `assetProfile` in the endpoint `GET api/v1/portfolio/holding/:dataSource/:symbol`
- Improved the language localization for German (`de`)
- Upgraded `svgmap` from version `2.19.3` to `2.21.0`

### Fixed

- Fixed a chart error on interaction by registering the annotation plugin early
- Fixed an issue on the allocations page where clicking an account in the _By Account_ chart did not open the detail dialog
- Restricted the maximum height of the import activities dialog
- Fixed the dark mode styling of the safe withdrawal rate selector in the _FIRE_ section (experimental)

### Special Thanks

- @dtslvr
- @jhernaezayuso
- @KenTandrian
- @MannXo

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.11.0

## Ghostfolio 3.11.0 Release Notes

### Added

- Added support for a click handler in the page tabs component

### Changed

- Improved the styling of the tabs across various dialogs
- Improved the styling of the page tabs component on desktop
- Enabled the _Bull Dashboard_ tab in the admin control panel (experimental)
- Migrated the settings dialog to customize the rule thresholds of the _X-ray_ page from `ngModel` to form control
- Improved the language localization for Spanish (`es`)
- Upgraded `bull-board` from version `7.1.5` to `7.2.1`
- Upgraded `date-fns` from version `4.1.0` to `4.4.0`

### Fixed

- Improved the loading state when customizing the rule thresholds on the _X-ray_ page

### Special Thanks

- @dtslvr
- @jhernaezayuso

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.10.0

## Ghostfolio 3.10.0 Release Notes

### Changed

- Improved the dynamic numerical precision for various values in the account detail dialog on mobile
- Improved the dynamic numerical precision for various values in the holding detail dialog on mobile
- Improved the account name display in the activities table
- Optimized the endpoint `GET api/v1/portfolio/holding/:dataSource/:symbol` by improving the processing of the historical market data

### Fixed

- Fixed an issue in the import dividends dialog
- Fixed an issue where certain symbols were incorrectly identified as currencies in various data providers
- Fixed the last request date in the users table of the admin control panel

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.9.0

## Ghostfolio 3.9.0 Release Notes

### Added

- Extended the _Public API_ with the endpoint to update the asset profile data (`PATCH api/v1/asset-profiles/:dataSource/:symbol`) (experimental)
- Added support for a dedicated _OpenRouter_ model for the `web_fetch` tool in the `FetchService`

### Changed

- Prefilled the form in the account balance management with the current cash balance
- Disabled the selection of future dates in the account balance management
- Grouped commodities and cryptocurrencies into the unknown bucket of the allocations by continent, country, currency, market and sector charts on the allocations page
- Moved the support for specific calendar year date ranges (`2025`, `2024`, `2023`, etc.) in the assistant from experimental to general availability
- Migrated various components from `NgStyle` to style bindings
- Improved the language localization for Korean (`ko`)

### Fixed

- Grouped activities without an account into the unknown bucket of the allocations by account and platform charts on the allocations page

### Special Thanks

- @battdir
- @DavidReque
- @dtslvr
- @Sjohn21
- @x52-dev

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.8.0

## Ghostfolio 3.8.0 Release Notes

### Added

- Added an automatic refresh every 30 seconds to the users table in the admin control panel

### Changed

- Harmonized the sector names across the data providers
- Localized the country names
- Localized the sector names
- Centralized the asset profile override logic for manual adjustments
- Improved the styling in the user detail dialog of the admin control panel’s users section
- Prevented the deletion of asset profiles that are currently in use
- Ensured market data is correctly removed when an asset profile with no remaining activities is deleted
- Refactored the backend logging to use the instance-based `Logger`
- Improved the language localization for German (`de`)
- Improved the language localization for Ukrainian (`uk`)

### Fixed

- Prevented the floating action button from overlapping the paginator on mobile
- Fixed an issue where the asset profile override (asset class and asset sub class) was not applied to the data enhancers when gathering asset profiles
- Fixed a layout issue in the asset profile dialog of the admin control panel by truncating long titles

### Special Thanks

- @dtslvr
- @KenTandrian
- @Punith1117
- @x52-dev

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.7.0

## Ghostfolio 3.7.0 Release Notes

### Added

- Added support for routing selected requests through the _OpenRouter_ `web_fetch` tool in the `FetchService`

### Changed

- Extended the countries mapping in the data enhancer for asset profile data via _Trackinsight_
- Removed the deprecated attributes (`assetClass`, `assetClassLabel`, `assetSubClass`, `assetSubClassLabel`, `countries`, `currency`, `dataSource`, `holdings`, `name`, `sectors`, `symbol` and `url`) from the holdings of the portfolio details endpoint response
- Upgraded `Nx` from version `22.7.2` to `22.7.5`

### Fixed

- Resolved an issue in the impersonation mode where the values did not match the owner’s currency
- Fixed the environment variable expansion in the `.env` file when debugging via _Visual Studio Code_

### Special Thanks

- @dtslvr
- @KenTandrian

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.6.0

## Ghostfolio 3.6.0 Release Notes

### Added

- Added `HTTP_PROXY`, `HTTPS_PROXY`, and `NO_PROXY` environment variable support to outbound HTTP requests
- Added the `FetchService` to centralize outbound HTTP requests

### Changed

- Extracted the floating action buttons (FAB) to a reusable component
- Upgraded `nestjs` from version `11.1.19` to `11.1.21`
- Upgraded `yahoo-finance2` from version `3.14.0` to `3.14.2`

### Special Thanks

- @DavidReque
- @dtslvr
- @gadicc
- @KenTandrian

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.5.0

## Ghostfolio 3.5.0 Release Notes

### Added

- Configured the `min-release-age` in `.npmrc`

### Changed

- Removed the deprecated attributes (`assetClass`, `countries`, `currency`, `dataSource`, `name`, `sectors`, `symbol` and `url`) from the holdings of the public portfolio endpoint response
- Removed the deprecated `api/v1/order` endpoints
- Upgraded `@keyv/redis` from version `4.4.0` to `5.1.6`

### Fixed

- Fixed a layout regression that caused a double scrollbar on pages without tabs
- Resolved an issue with missing cash positions caused by an incorrect data source

### Special Thanks

- @dtslvr
- @KenTandrian
- @Trillianti

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.4.0

## Ghostfolio 3.4.0 Release Notes

### Added

- Added the icon column to the benchmark component
- Added support for the `DIRECT_URL` environment variable to enable direct database connections

### Changed

- Improved the pagination in the activities table of the account detail dialog
- Improved the pagination in the activities table of the holding detail dialog
- Randomized the placeholder in the assistant
- Filtered out sectors with zero weight for ETF and mutual fund assets in the _Yahoo Finance_ data enhancer
- Enabled the _Bull Dashboard_ in the admin control panel without requiring an environment variable (experimental)
- Improved the verification of the _Stripe_ checkout session when creating a subscription
- Relaxed the URL validation in the asset profile DTOs to accept both `HTTP` and `HTTPS` protocols
- Relaxed the URL validation in the platform DTOs to accept both `HTTP` and `HTTPS` protocols
- Extracted the page tabs to a reusable component
- Improved the language localization for German (`de`)
- Improved the language localization for Spanish (`es`)
- Upgraded `bull-board` from version `7.0.0` to `7.1.5`
- Upgraded `Nx` from version `22.7.1` to `22.7.2`

### Fixed

- Resolved an issue with the cash balance calculation of an account for `SELL` activities to ensure fees are correctly subtracted
- Resolved an exception in the portfolio details endpoint when an asset profile is unmatched

### Special Thanks

- @ccfiel
- @dtslvr
- @jhernaezayuso
- @KenTandrian
- @lil-goat

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.3.0

## Ghostfolio 3.3.0 Release Notes

### Added

- Added `nestjs-best-practices` skills

### Changed

- Deactivated asset profiles automatically on delisting in the _Financial Modeling Prep_ service
- Migrated various components from `NgClass` to class bindings
- Refreshed the cryptocurrencies list
- Improved the language localization for Spanish (`es`)
- Cleaned up the _Webpack Bundle Analyzer_ setup
- Upgraded `@internationalized/number` from version `3.6.5` to `3.6.6`
- Upgraded `@ionic/angular` from version `8.8.1` to `8.8.5`
- Upgraded `@openrouter/ai-sdk-provider` from version `0.7.2` to `2.9.0`
- Upgraded `ai` from version `4.3.16` to `6.0.174`
- Upgraded `bull-board` from version `6.20.3` to `7.0.0`
- Upgraded `countries-and-timezones` from version `3.8.0` to `3.9.0`
- Upgraded `fuse.js` from version `7.1.0` to `7.3.0`
- Upgraded `Nx` from version `22.6.5` to `22.7.1`
- Upgraded `papaparse` from version `5.3.1` to `5.5.3`
- Upgraded `prisma` from version `7.7.0` to `7.8.0`

### Fixed

- Synchronized the native browser elements with the theme to improve the dark mode
- Fixed a visual regression in the bottom navigation bar on mobile

### Special Thanks

- @DavidReque
- @dtslvr
- @jhernaezayuso
- @KenTandrian

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.2.0

## Ghostfolio 3.2.0 Release Notes

### Added

- Added `angular-developer` skills

### Changed

- Harmonized the unit styling in the value component
- Upgraded `stripe` from version `20.4.1` to `21.0.1`

### Fixed

- Resolved a validation error with an empty URL in the asset profile details dialog of the admin control panel
- Resolved an issue where charts and components defaulted to _Roboto_ instead of the preconfigured _Inter_ font family

### Special Thanks

- @dtslvr
- @KenTandrian

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.1.0

## Ghostfolio 3.1.0 Release Notes

### Added

- Added the _EuroAlternative_ logo to the logo carousel on the landing page
- Integrated a theme switcher into _Storybook_ to support toggling between the light and dark mode

### Changed

- Modernized the layout of the overview tab in the admin control panel
- Improved the styling of the paginator across various table components
- Improved the language localization for German (`de`)

### Fixed

- Optimized the spacing of the logo in the header
- Fixed the _Storybook_ setup by resolving missing `@angular/material` styles

### Special Thanks

- @DavidReque
- @dtslvr
- @lechtidu56
- @mvanhorn

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 3.0.1

## Ghostfolio 3.0.1 Release Notes

### Changed

- Moved the copy-to-clipboard button for the ISIN number in the holding detail dialog from experimental to general availability
- Moved the copy-to-clipboard button for the symbol in the holding detail dialog from experimental to general availability
- Improved the styling of buttons and input fields across various components
- Upgraded `prettier` from version `3.8.2` to `3.8.3`

### Fixed

- Fixed the cash label in the holdings table of the portfolio holdings page
- Fixed the cash label in the holdings table of the public page

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# v3.0.0.1 - Startup Crash Fix

### Fixed:

Resolved an issue where the add-on would enter a continuous crash loop upon updating to Ghostfolio 3.0.0.

# 3.0.0

## Ghostfolio 3.0.0 Release Notes

### Added

- Added a blog post: _Announcing Ghostfolio 3.0_

### Changed

- Migrated from _Material Design_ 2 to _Material Design_ 3
- Moved the total amount, change and performance with currency effects on the analysis page from experimental to general availability
- Refreshed the cryptocurrencies list
- Upgraded `countup.js` from version `2.9.0` to `2.10.0`
- Upgraded `jsonpath` from version `1.2.1` to `1.3.0`
- Upgraded `nestjs` from version `11.1.14` to `11.1.19`
- Upgraded `ngx-markdown` from version `21.1.0` to `21.2.0`
- Upgraded `Nx` from version `22.6.4` to `22.6.5`
- Upgraded `prisma` from version `6.19.0` to `7.7.0`

### Todo

- **Breaking Change**: The `sslmode=prefer` parameter in `DATABASE_URL` is no longer supported. Please update your environment variables (see `.env`) to use `sslmode=require` if _SSL_ is enabled or remove the `sslmode` parameter entirely if _SSL_ is not used.

### Special Thanks

- @dtslvr
- @KenTandrian

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 2.255.0

## Ghostfolio 2.255.0 Release Notes

### Changed

- Sorted the activity types alphabetically on the activities page (experimental)
- Sorted the asset classes of the assistant alphabetically
- Sorted the tags of the assistant alphabetically
- Upgraded `angular` from version `21.1.1` to `21.2.7`
- Upgraded `Nx` from version `22.5.3` to `22.6.4`
- Upgraded `prettier` from version `3.8.1` to `3.8.2`
- Upgraded `svgmap` from version `2.19.2` to `2.19.3`
- Upgraded `yahoo-finance2` from version `3.13.2` to `3.14.0`

### Fixed

- Fixed the missing value column of the accounts table component on mobile

### Special Thanks

- @DavidReque
- @dtslvr
- @Horvath-Fabian
- @jacobbjelkekachel
- @KenTandrian

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 2.254.0

## Ghostfolio 2.254.0 Release Notes

### Added

- Added loan as an asset sub class

### Changed

- Extended the asset profile details dialog in the admin control panel to support editing countries for all asset types
- Extended the asset profile details dialog in the admin control panel to support editing sectors for all asset types
- Migrated the data collection for the _Open Startup_ (`/open`) page to the queue design pattern
- Improved the language localization for German (`de`)
- Upgraded `lodash` from version `4.17.23` to `4.18.1`

### Fixed

- Improved the style of the activity type component

### Special Thanks

- @dtslvr
- @Erwin-N
- @KenTandrian
- @omkarg01

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 2.253.0

## Ghostfolio 2.253.0 Release Notes

### Added

- Added support for filtering by activity type on the activities page (experimental)
- Extended the admin control panel by adding a copy-to-clipboard button for the application version

### Changed

- Extended the terms of service for the _Ghostfolio_ SaaS (cloud) to include _Paid Plans_ and _Refund Policy_
- Upgraded `prisma` from version `6.19.0` to `6.19.3`

### Fixed

- Fixed the allocations by account chart on the allocations page in the _Presenter View_
- Fixed the allocations by asset class chart on the allocations page in the _Presenter View_
- Fixed the allocations by currency chart on the allocations page in the _Presenter View_
- Fixed the allocations by ETF provider chart on the allocations page in the _Presenter View_
- Fixed the allocations by platform chart on the allocations page in the _Presenter View_

### Special Thanks

- @Airthee
- @DavidReque
- @dtslvr
- @Erwin-N
- @KenTandrian
- @tmchow

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 2.252.0

## Ghostfolio 2.252.0 Release Notes

### Added

- Added support for a copy-to-clipboard functionality in the value component
- Extended the holding detail dialog by adding a copy-to-clipboard button for the ISIN number (experimental)
- Extended the holding detail dialog by adding a copy-to-clipboard button for the symbol (experimental)
- Extended the user detail dialog of the admin control panel’s users section by adding a copy-to-clipboard button for the user id

### Changed

- Refreshed the cryptocurrencies list
- Improved the language localization for German (`de`)
- Improved the language localization for Spanish (`es`)
- Upgraded `countries-list` from version `3.2.2` to `3.3.0`
- Upgraded `ng-extract-i18n-merge` from `3.2.1` to `3.3.0`
- Upgraded `stripe` from version `20.3.0` to `20.4.1`

### Special Thanks

- @AyushMishraa
- @dtslvr
- @Erwin-N
- @jhernaezayuso
- @KenTandrian

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 2.251.0

## Ghostfolio 2.251.0 Release Notes

### Added

- Added the quantity column to the holdings table of the portfolio holdings page

### Changed

- Hardened the endpoint `DELETE /api/v1/auth-device/:id` by improving the user validation
- Improved the allocations by ETF holding on the allocations page by refining the grouping of the same assets with diverging names (experimental)
- Improved the language localization for Polish (`pl`)
- Upgraded `@trivago/prettier-plugin-sort-imports` from version `5.2.2` to `6.0.2`

### Fixed

- Fixed an issue by adding a missing guard in the public access for portfolio sharing

### Special Thanks

- @BoB5231
- @dtslvr
- @Erwin-N
- @KenTandrian
- @mvanhorn
- @NathanDrake2406
- @omkarg01

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 2.250.0

## Ghostfolio 2.250.0 Release Notes

### Added

- Added support for specific calendar year date ranges (`2025`, `2024`, `2023`, etc.) on the portfolio activities page

### Changed

- Consolidated the sign-out logic within the user service to unify cookie, state and token clearance
- Improved the language localization for Polish (`pl`)
- Upgraded `@ionic/angular` from version `8.7.3` to `8.8.1`
- Upgraded `replace-in-file` from version `8.3.0` to `8.4.0`
- Upgraded `svgmap` from version `2.14.0` to `2.19.2`
- Pinned the _Node.js_ version in the _Build code_ _GitHub Action_ to ensure environment consistency for tests

### Fixed

- Fixed an issue with the detection of the thousand separator for the `de-CH` locale
- Fixed an issue in the _Storybook_ stories of the symbol autocomplete component caused by a circular dependency

### Special Thanks

- @Akd11111
- @AyushMishraa
- @dtslvr
- @Erwin-N
- @gilangjavier
- @JiwaniZakir
- @KenTandrian
- @mvanhorn
- @NathanDrake2406
- @WinnCook

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 2.249.0

## Ghostfolio 2.249.0 Release Notes

### Added

- Integrated _Bull Dashboard_ for a detailed jobs queue view in the admin control panel (experimental)
- Added a debounce to the `PortfolioChangedListener` and `AssetProfileChangedListener` to minimize redundant _Redis_ and database operations

### Changed

- Improved the _Storybook_ stories of the value component
- Improved the language localization for Dutch (`nl`)
- Improved the language localization for German (`de`)
- Upgraded `class-validator` from version `0.14.3` to `0.15.1`

### Fixed

- Fixed false _Redis_ health check failures by using unique keys and increasing the timeout to 5s

### Special Thanks

- @dtslvr
- @Erwin-N

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 2.248.0

## Ghostfolio 2.248.0 Release Notes

### Added

- Added support for column sorting to the data providers management of the admin control panel

### Changed

- Included asset profile data in the endpoint `GET api/v1/portfolio/holdings`
- Included asset profile data in the holdings of the public page
- Reused the value component in the platform management of the admin control panel
- Reused the value component in the tag management of the admin control panel
- Deprecated the `api/v1/order` endpoints in favor of the `api/v1/activities` endpoints
- Upgraded `jsonpath` from version `1.1.1` to `1.2.1`

### Fixed

- Fixed an issue in the _FIRE_ calculator to correctly calculate the projected total amount

### Special Thanks

- @DarkwinngDuck
- @DavidReque
- @dtslvr
- @KenTandrian
- @WinnCook

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 2.247.0

## Ghostfolio 2.247.0 Release Notes

### Changed

- Upgraded `yahoo-finance2` from version `3.13.0` to `3.13.2`

### Special Thanks

- @dtslvr
- @gadicc
- @lmaced0

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 2.246.0

## Ghostfolio 2.246.0 Release Notes

### Changed

- Removed the deprecated `committedFunds` from the summary of the portfolio details endpoint
- Upgraded `Nx` from version `22.4.5` to `22.5.3`

### Fixed

- Fixed an issue where the apply and reset filter buttons remained disabled in the assistant

### Special Thanks

- @DarkwinngDuck
- @dtslvr
- @pswitchy
- @slegarraga

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 2.245.0

## Ghostfolio 2.245.0 Release Notes

### Changed

- Excluded the scraper configuration from the import and export functionality
- Excluded the symbol mapping from the import and export functionality
- Improved the language localization for Dutch (`nl`)
- Improved the language localization for Italian (`it`)
- Improved the language localization for Spanish (`es`)

### Fixed

- Resolved the data source transformation in the errors of the performance endpoint
- Resolved the data source transformation in the export functionality

### Special Thanks

- @arielpons
- @dtslvr
- @Erwin-N
- @ratrarity
- @riccobelli

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 2.244.0

## Ghostfolio 2.244.0 Release Notes

### Changed

- Improved the usability of the asset profile details dialog in the admin control panel for currencies
- Removed the deprecated static portfolio analysis rule: _Fees_ (Fee Ratio)
- Refactored queries in the data provider service to use Prisma’s safe query methods

### Fixed

- Fixed an exception by adding a fallback for missing market price values on the _X-ray_ page

### Special Thanks

- @agarg5
- @dtslvr
- @KenTandrian
- Aidan Crinion

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 2.243.0

## Ghostfolio 2.243.0 Release Notes

### Changed

- Improved the language localization for Chinese (`zh`)
- Upgraded `nestjs` from version `11.1.8` to `11.1.14`

### Fixed

- Fixed an issue when creating activities of type `FEE`, `INTEREST` or `LIABILITY`

---
*This release was automatically generated based on the official Ghostfolio update.*

---

# 2.243.0

## Ghostfolio 2.243.0 Release Notes

### Changed

- Improved the language localization for Chinese (`zh`)
- Upgraded `nestjs` from version `11.1.8` to `11.1.14`

### Fixed

- Fixed an issue when creating activities of type `FEE`, `INTEREST` or `LIABILITY`

---
*This release was automatically generated based on the official Ghostfolio update.*

---

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
