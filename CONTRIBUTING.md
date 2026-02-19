# Contributing Guide

Thank you for contributing to the DevOps Hybrid Lab.

## Branching Model

- Use short-lived feature branches from `main`
- Open pull requests for all changes
- Keep each PR focused on one infrastructure concern

## Commit Messages

Use clear, action-oriented commits.

Suggested prefixes:

- `feat:` new functionality
- `fix:` bug fix
- `docs:` documentation updates
- `chore:` maintenance tasks
- `refactor:` internal improvements

## Pull Request Expectations

- Include objective and affected environment(s)
- Include `plan` output summary for Terraform changes
- Include Ansible run evidence for config changes
- Update docs when topology/process changes

## Quality Checks

Before opening a PR:

1. Run Terraform format and validation
2. Review Terraform plan output
3. Execute Ansible syntax/idempotency checks where applicable

## Security and Secrets

- Do not commit cloud credentials or private keys
- Use remote state with locking for Terraform
- Apply least-privilege access principles
