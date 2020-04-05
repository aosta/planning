# AOSTA

## Mission

The mission is to build out AWS infrastructure for deploying a sample Wordpress site.
This is to be used as an exemplar of modern IaC design patterns and tooling.

## Principles

### Architectural Decision Records

Keep a simple ADR to track decisions around tooling or other patterns.

* Architecturial Decision Register
  * https://adr.github.io/madr/

### Terraform Modules

* Have a central set of terraform modules that can be composed into a working infrastructure.
  * semver
  * no monorepo
  * CI pipelines
    * tests
    * lint
    * docs

### IaC

* Use Terragrunt to DRY up the IaC
* Consume modules from the AOSTA module library
  * Fork Hashicorp trusted modules where ever possible
  * contribute back changes
* Treat as code and follow good SDLC practices

