# Contributing to iNAYASearch

Thank you for your interest in contributing to iNAYASearch.

iNAYASearch is an open-source web search engine being developed by iNAYATechLab. The project aims to build its own search infrastructure and core retrieval technology incrementally, with a strong focus on correctness, security, performance, privacy, and maintainability.

## Before You Start

Please read the following documents before making a contribution:

- `README.md` — Project overview
- `ROADMAP.md` — Development roadmap
- `SECURITY.md` — Security policy
- `CODE_OF_CONDUCT.md` — Community standards

Do not make large architectural changes without first discussing them with the maintainers.

## Development Philosophy

iNAYASearch follows a staged engineering process:

1. Inspect
2. Design
3. Implement
4. Test
5. Security Review
6. Performance Review
7. Document
8. Phase Sign-off
9. Continue to the next phase

Changes should be small, understandable, testable, and documented.

## Core Search Technology

The core search technology of iNAYASearch is intended to be developed by the project itself.

Core components include:

- URL canonicalization
- URL validation
- Web crawling
- URL frontier and scheduling
- HTML parsing and content extraction
- Tokenization and normalization
- Inverted indexing
- Query processing
- Retrieval
- Ranking
- BM25 scoring
- Search quality evaluation

Third-party hosted search engines or search APIs should not be used as the core search engine.

Supporting infrastructure and standard development tools may be used when appropriate.

## Repository Structure

The project is organized into major areas such as:

- `apps/` — User-facing applications
- `services/` — Search services
- `packages/` — Shared and core libraries
- `infrastructure/` — Deployment and infrastructure configuration
- `docs/` — Technical documentation
- `tests/` — Test suites
- `.github/` — GitHub project configuration

The structure may evolve as the project develops.

## Issues

Before opening an issue:

1. Check whether the issue already exists.
2. Make sure the issue is reproducible when reporting a bug.
3. Provide enough technical information to understand the problem.
4. Avoid including secrets, credentials, tokens, or private information.

Use the appropriate issue template whenever available.

## Feature Requests

Feature requests should explain:

- What problem the feature solves
- Why the feature is useful
- How it could fit into the existing architecture
- Any relevant performance or security considerations

Large features should be discussed before implementation.

## Pull Requests

Pull Requests should:

- Have a clear and concise title.
- Explain what was changed.
- Explain why the change was necessary.
- Include relevant tests.
- Avoid unrelated changes.
- Avoid committing secrets or credentials.
- Update documentation when necessary.
- Follow the project's coding and architectural conventions.

A Pull Request may be reviewed for:

- Correctness
- Security
- Performance
- Maintainability
- Test coverage
- API and data compatibility
- Architectural consistency

## Commit Messages

Use clear and descriptive commit messages.

Preferred format:

```text
type: short description