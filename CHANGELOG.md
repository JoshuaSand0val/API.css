# Changelog

All relevant changes to API.css will be documented here.

## [1.0.0-beta.3] - 2023-03-10

### Added

- Added root `_index.scss` as an accessible entry point into API.css.
- Added `size` shorthand mixin for using the `size()` function across breakpoints.
- Added `prefers-motion` media query mixin for when the user requests motion.

### Changed

- Changed `font-size` mixin parameter name from `$values` to intended `$steps`.
- Changed `breakpoints` mixin by removing `$properties`, and to only accept `$values`.

## [1.0.0-beta.2] - 2023-03-04

### Added

- Added `font-size` shorthand mixin for setting typography size across viewport breakpoints.
- Added `@content` block support to `breakpoints` mixin.
- Added functionality to `shade` and `tint` functions. They now can accept an integer for `$perc` to multiply their output by a fixed `$color-shift` percentage value.

### Changed

- Changed `color-shift` function to use `luminance` (opposed to SASS `lightness` function).

### Fixed

- Fixed `declare` mixin from outputting `null` properties.

## [1.0.0-beta.1] - 2023-01-08

### Added

- Added `$z-underlay` and `$z-overlay` Z-Index variables.
- Added `$safe-header` and `$safe-footer` safe-area variables.
- Added use of `null` keyword to skip breakpoint in `breakpoints()` mixin.

### Changed

- Changed variable `$z-modal-backdrop` name to `$z-backdrop`.
- Changed variable `$z-popover` name to `$z-popup`.
- Changed Z-Index variable defaults to reflect added variables.
- Changed variable `$vw-map` name to `$viewports`.

## [1.0.0-beta.0] - 2022-12-28

### Added

- Initial beta release (cloned from Neo CSS preview branch).

[1.0.0-beta.3]: https://github.com/JoshuaSand0val/API.css/releases/tag/v1.0.0-beta.3
[1.0.0-beta.2]: https://github.com/JoshuaSand0val/API.css/releases/tag/v1.0.0-beta.2
[1.0.0-beta.1]: https://github.com/JoshuaSand0val/API.css/releases/tag/v1.0.0-beta.1
[1.0.0-beta.0]: https://github.com/JoshuaSand0val/API.css/releases/tag/v1.0.0-beta.0