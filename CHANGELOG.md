# Release Notes for Abandoned Cart

## 1.3.4 - 2019-08-05
### Fixed
- Removed cart variable from default example templates. Users using the default templates were experiencing issues with sessions

## 1.3.3 - 2019-08-05
### Changed
- Updated dashboard to show last updated date from the order and not the abandoned cart record
- Added order reference to dashboard table

## 1.3.2 - 2019-07-10
### Fixed
- Fixed an issue where test mode was not set on the dashboard when no orders have yet been abandoned

## 1.3.1 - 2019-07-04
### Fixed
- Fixed an issue on the dashboard where the order wasn't being found and displayed

### Changed
- Dashboard now displays if Test Mode is enabled or not
- If cart recovery fails (expired) and a custom recovery url is set, that will be used

## 1.3.0 - 2019-06-08
### Added
- Jobs can be triggered via a URL now using a secret key. This means people without access to cron jobs can use this plugin
- Added setting for a configurable secret key which is used to verify job requests

## 1.2.0 - 2019-06-08
### Added
- Test Mode 🎉 Test mode allows the queue to be bypassed and emails to instantly be sent allowing for quicker and easier testing
- Default email templates now include `{% set cart = craft.commerce.carts.cart %}` so that commerce helper functions like `|currency` can be used

## 1.1.6 - 2019-06-04
### Added
- Added support for `allowAdminChanges`, settings will be disabled by default

## 1.1.5 - 2019-05-30
### Changed
- New plugin icon 🎉

### Fixed
- Fixed the issue [#14] which involved abandoned carts with no email addresses. I've submitted a pull request to Craft Commerce to change how emails are stored when an order is first created

[#14]: https://github.com/mediabeastnz/craft-commerce-abandoned-cart/issues/14

## 1.1.4 - 2019-05-19
### Fixed
- Resolved a date deprecation warning

## 1.1.3 - 2019-05-10
### Fixed
- Abandoned carts still display if original Order is missing

## 1.1.2.1 - 2019-04-10
### Fixed
- Patch for last version, fixes missing folder

## 1.1.2 - 2019-04-10
### Fixed issue [#4]
- Fixed a bug that was introduced in version 1.1.1

[#4]: https://github.com/mediabeastnz/craft-commerce-abandoned-cart/issues/4

### Added
- Added the ability to change recovery url to soemthing other than shop/cart

## 1.1.1 - 2019-03-23
### Added
- Added pagination to the dashboard to handle sites with large amounts of orders

## 1.1.0 - 2019-03-19
### Added
- You can now manually trigger the job that searches for abandoned carts! Useful if you don't have access to cron jobs
- Added additional documention/instructions to help with setup

## 1.0.1 - 2019-02-20
### Fixed
- Breadcrumb link

## 1.0.0 - 2019-02-16
### Added
- Initial release
