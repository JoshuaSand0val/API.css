# Changelog

All relevant changes to API.css will be documented here.

## [1.0.0-beta.5] - 2023-05-27

### Added

- Added API forward in optional starter stylesheet.
- Added `states` mixin to spread values across selectors.
- Added `color-weight` function to weight color lightness.
- Added `$primary-color` variable, and `primary-color` mixin.
- Added `legible-color` mixin for setting type color.
- Added `accent` to `$colors` map.

### Changed

- Changed starter stylesheet in moving html properties into body. This allows the styles to be wrapped in a class for CSS modules support, if needed.
- Changed `color-shift`, `shade` and `tint` functions syntax from percentages to color weights.
- Changed `$color-scheme` variable name to `$color-schemes`.
- Changed optional starter stylesheet to use new color mixins.
- Changed `color-schemes` mixin functionality to omit its output based off its corresponding `$color-schemes` variable.

### Removed

- Removed inset mixin in favor of the native CSS property instead.
- Removed `state` mixin in favor of new `states` mixin.
- Removed `!default` configuration on `$colors`, `$viewports` and `$breakpoints`.
- Removed `$background-color` variable and `background-color` mixin.
- Removed `$color-shift` percentage variable.
- Removed `step-color` function and `$contrast-step-ratio` variable.
- Removed `text-color` function and `$contrast-text-ratio` variable.
- Removed `tone` function.

## [1.0.0-beta.4] - 2023-03-15

### Added

- Added `$color-shift` multiplying integer syntax to `tone` function.
- Added `@content` block support to `font-size` mixin.
- Added `state` mixin that includes `$true` and/or `$false` state for a given `$selector`.
- Added `$accent` color variable default.
- Added optional `/scss/styles/` stylesheet that brings over API defaults to HTML elements, as well as useful defaults to preserve page responsiveness.
- Added `$time-xs`, `$time-sm`, `$time-md`, `$time-lg`, `$time-xl` and `$time-xxl` variable defaults for transitions/animations.

### Changed

- Changed `$perc` syntax of `shade` and `tint` functions to `$amount`.
- Changed `$font-size-ratio` default to `1.250` from `1.200`.

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

[1.0.0-beta.5]: https://github.com/JoshuaSand0val/API.css/releases/tag/v1.0.0-beta.5
[1.0.0-beta.4]: https://github.com/JoshuaSand0val/API.css/releases/tag/v1.0.0-beta.4
[1.0.0-beta.3]: https://github.com/JoshuaSand0val/API.css/releases/tag/v1.0.0-beta.3
[1.0.0-beta.2]: https://github.com/JoshuaSand0val/API.css/releases/tag/v1.0.0-beta.2
[1.0.0-beta.1]: https://github.com/JoshuaSand0val/API.css/releases/tag/v1.0.0-beta.1
[1.0.0-beta.0]: https://github.com/JoshuaSand0val/API.css/releases/tag/v1.0.0-beta.0