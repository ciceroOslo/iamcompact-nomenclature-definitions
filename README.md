# iamcompact-nomenclature-definitions
Nomenclature definitions for iamcompact-nomenclature (additions or overrides to common-definitions)


## Purpose and connection with other repositories

This repository contains codelists for the IAM COMPACT project that are
compatible with the `nomenclature-iamc` Python package. It is used by the
packages `iamcompact-nomenclature` and `iamcompact-validation-ui` for validating
model, scenario, variable and region names and units, and for defining
aggregation mappings between regions.

Definitions of variables in this repository come in addition to or override ones
given in the `common-definitions` repository. Definitions from
`common-definitions` are stored in a fork of the official `common-definitions`
repository, at [https://github.com/ciceroOslo/common-definitions/](https://github.com/ciceroOslo/common-definitions/)
(the official repo is at
[https://github.com/IAMconsortium/common-definitions](https://github.com/IAMconsortium/common-definitions)).
The definitions used in IAM COMPACT are taken from the branches
`iamcompact-definitions-main` and `iamcompact-validation-ui`. These are
generally kept up to date with the main branch of `common-definitions`, but may
be frozen at some point, or may be kept back for testing or in the case of
compatibility issues that arise with new changes.


## Organization

Codelist definitions are stored in the `/definitions/` folder, and region
mappings in the `/mappings/` folder, like for any `nomenclature` definitions
repository.

Each of these folders contain a subfolder named `common-definitions-overrides`,
which contains definitions that override existing definitions in
`common-definitions`. These subfolders generally mirror the subfolder structures
and file names in the `common-definitions` repository. Files and subfolders
outside of `common-definitions-overrides` are additional definitions that are
not present in `common-definitions`.

The `main` branch of this repository is the master version of the recommended
names and mappings for use in IAM COMPACT. The GUI validation app/web app (at
[https://github.com/ciceroOslo/iamcompact-validation-ui](https://github.com/ciceroOslo/iamcompact-validation-ui))
uses definitions from the branch `validation-ui`. This branch is usually kept in
sync with `main`, but may differ or be delayed in the case of technical issues
arising from newly added definitions.
