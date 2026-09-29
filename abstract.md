# Administering R: Installations, Libraries, and Package Management

**Format:** 4-hour virtual workshop
**Audience:** System administrators and platform engineers supporting R users

This workshop looks at how shared R environments are installed, configured, and updated, and gives system administrators a practical, end-to-end model of how R finds and loads packages, and how to control that on a shared server.

We start with the anatomy of an R installation: how `R` and `Rscript` differ, and how site-wide configuration (`Rprofile.site`, `Renviron.site`) shapes every session your users start. From there we work through the default, site, and user libraries, and how `.libPaths()` resolves them. We then discuss how to deal with CRAN, Bioconductor, and internal package repositories.

The second half is about installing packages predictably. We cover R's dependency types (Depends, Imports, LinkingTo, Suggests), resolving system dependencies with `r-system-requirements` and `pak`, and building a local repository as a stable, snapshot-able source of truth. We then test a package set as a cohort with `R CMD check` before release, install it with `install.packages()`, and close with incremental maintenance using `update.packages()` and `remove.packages()`.

There will also be time to discuss real-world production issues as a group. Attendees leave with a foundation to stand up, test, and incrementally maintain an R environment for their organization.

## Topics

- R installation, site configuration, `R` vs. `Rscript`
- CRAN, Bioconductor, and internal packages; default, site, and user libraries; `.libPaths()`
- Dependency management: Depends, Imports, LinkingTo, Suggests
- System dependencies: `r-system-requirements` and `pak`
- Building a local repository
- Cohort testing with `R CMD check`
- Installing packages with `pak` and `install.packages()`
- Incremental package installation: `install.packages()`, `update.packages()`, `remove.packages()`
