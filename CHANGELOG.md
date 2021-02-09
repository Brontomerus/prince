# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.7.1] - 2021-01-29

### Added

- error handing to catch cases someone has not installed prince[plot], and does not have matplotlib.
- documentation added to reflect the new installation changes.

### Changed

- adjusted matplotlib dependencies to enable optional installs [@brontomerus](https://github.com/brontomerus).

## 0.7.0

- `prince` is now compatible with `pandas>=1.0`.

### Added

- `PCA` now has an `inverse_transform` function.

### Changed

- `MFA` and `FAMD` should now be able to `fit` and `transform` on categorical variables with different number of distinct values.
- Fixed a bug where `column_correlations` would raise an `AttributeError` in a `FAMD`.
- The output of `column_correlations` is now sorted along the index.
