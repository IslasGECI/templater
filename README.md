<a href="https://www.islas.org.mx"><img src="https://www.islas.org.mx/img/logo.svg" align="right" width="256" /></a>

# Template for R projects
[![codecov](https://codecov.io/gh/IslasGECI/templater/graph/badge.svg?token=wyxnwZypMA)](https://codecov.io/gh/IslasGECI/templater)
![example branch
parameter](https://github.com/IslasGECI/templater/actions/workflows/actions.yml/badge.svg)
![licencia](https://img.shields.io/github/license/IslasGECI/templater)
![languages](https://img.shields.io/github/languages/top/IslasGECI/templater)
![commits](https://img.shields.io/github/commit-activity/y/IslasGECI/templater)
![R-version](https://img.shields.io/github/r-package/v/IslasGECI/templater)

## Steps to create a new project from this template

> **Note:** For `NEW_R_PACKAGE_NAME`, use all lowercase with no separators (no underscore, no dot, no CamelCase).
> Example: if repo name is `seabird_tracking`, use `seabirdtracking`.

1. **README.md** (2 changes)
   - Replace `IslasGECI/templater` → `IslasGECI/<NEW_PROJECT_NAME>`
   - Replace codecov token `?token=wyxnwZypMA` → `<NEW_PROJECT_TOKEN>`

2. **CHANGELOG.md** (1 change)
   - Replace `github.com/IslasGECI/templater` → `github.com/IslasGECI/<NEW_PROJECT_NAME>`

3. **docker-compose.yml** (1 change)
   - Replace `islasgeci/templater` → `islasgeci/<NEW_PROJECT_NAME>`

4. **DESCRIPTION** (1 change)
   - Replace `Package: templater` → `Package: <NEW_R_PACKAGE_NAME>`

5. **.github/workflows/actions.yml** (7 changes)
   - Replace all `islasgeci/templater` → `islasgeci/<NEW_PROJECT_NAME>`

6. **tests/testthat.R** (2 changes)
   - Replace `library(templater)` → `library(<NEW_R_PACKAGE_NAME>)`
   - Replace `test_check("templater")` → `test_check("<NEW_R_PACKAGE_NAME>")`

7. **tests/testthat/test_nothing.R** (1 change)
   - Replace `packageVersion("templater")` → `packageVersion("<NEW_R_PACKAGE_NAME>")`

8. **tests/testthat/coverage.R** (1 change)
   - Replace codecov token `53631a87-1660-47ba-a000-789a8b05283f` → `<NEW_PROJECT_TOKEN>`

### Verification
Run `grep -r "templater" .` to confirm no instances remain.
