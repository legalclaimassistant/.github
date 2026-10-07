# GitHub Templates & configuration

This repository contains standardized templates and GitHub configurations for our organization.  
It ensures that all repositories have consistent defaults for issues, pull requests, and automated workflows.

## What's included

- **Issue & PR templates** – standardized templates for consistent reporting and reviews.  
- **GitHub Actions** – automation scripts for CI/CD and other tasks.  
- **CODEOWNERS** – define repository maintainers and automatic reviewers.  
- **Other repository defaults** – such as labels, funding, and security policies.

## Shared configuration

- **`.github/release-drafter.yml`** – the release-drafter configuration for every repository. A repository opts in with a `.github/release-drafter.yml` containing only `_extends: .github`, and may override individual keys below that line. Tags have no `v` prefix (e.g. `0.12.0`).

## How it works

Files in this repository act as **defaults** for every repository in the organization.  
If a repository contains its own version of a template, workflow, or configuration file, it will **override** the default from this repo.

## Why

Centralizing templates and workflows ensures that all repositories:

- Follow the same standards.  
- Are easier to manage and maintain.  
- Provide clear guidance for contributors and maintainers.

