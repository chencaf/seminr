# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]
- Change code syntax to remove interactions() method and add interactions and HOC to composites()
- Document all the syntax and features

## [1.0.1] - 2019-12-11
### Changed
- Patched if() conditionals including class() to reflect new CRAN class of matrix as c("matrix","array") in R V4.0.0

## [0.1.0] - 2019-09-27
### Added
- A changelog
- A new feature for automated calculation of HOC
- A new feature for two-stage calculation of interactions
- A file for all references and citations
- A return object in summary(boot_seminr_model) containing boot mean, SD, tvalue, and CIs for bootstrapped paths, loadings, weights and HTMT, 
- A test for the bootstrap summary return object
- Descriptive statistics for item and construct data
- S3 print method for class "table_output" for printing generic tables
- new method interaction_term() for specifying a interaction construct
- A fSquare function to calculating fSquared
- A test for fSquared function

### Changed
- Fixtures for evaluating bootstrap HTMT for versions of R < 3.6.0
- Changed the R/* file naming to R/estimate_ R/feature_ R/evaluate_ etc.
- Summary S3 method to return data descriptives in summary object
- constructs() method now returns a list with classes
- Changed references to include Cohen (2013)
- Updated vignette to reflect fSquare function

### Fixed
- Modified calculation of HTMT to use absolute correlation matrices in order to make HTMT stable
