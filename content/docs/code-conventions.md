+++
author = "kenjitheman"
title = "Code Conventions"
date = "2023-12-27"
description = "Here is explanation of our code conventions."
tags = [
    "text",
    "docs",
    "help",
    "guide"
]
+++

# Code Conventions

> The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](https://www.rfc-editor.org/rfc/rfc2119).

## Priority values

- `Low` - low priority (small pinpoint improvements)
- `Normal` - normal priority (main features, fixes)
- `High` - high priority (more important main feature, fix)
- `Blocker` - other tasks can't be performed until this issue is resolved

## Estimation values

- `Hours` - an issue might take 1-8 hours
- `Days` - an issue might take 1-7 days
- `Weeks` - an issue might take 1-2 weeks

If estimation exceeds 2 weeks, an issue MUST be split into smaller ones.

## Repository rules

- A repository MUST NOT allow `merge commits`.
- A repository MUST NOT allow `squash merging`.
- A repository MUST only allow `rebase merging`.

## Branch rules

- A main branch name MUST be `master`.
- A master branch name MUST be protected.
- A master branch name MUST NOT be force pushed.
- A new branch MUST be created for each issue or feature.
- A new branch name MUST follow the next pattern `<type>/PR-NUMBER/optional-info`, where `<type>` is from [Conventional Commits v1.0.0](https://www.conventionalcommits.org/en/v1.0.0/) standard.

  > e.g. 
  > - fix/#9
  > - feat/#883/hatsune-miku-the-real-one
  > - docs/#1/me-and-waifu

## Commit rmaster

- A commit message MUST follow [Conventional Commits v1.0.0](https://www.conventionalcommits.org/en/v1.0.0/) standard.
- A commit message MUST contain the pull request number (e.g., #54) in a scope.
  
  > e.g. `fix(#53): change button color to red`
- A commit SHOULD be signed off.

## Issue rules

- If an issue is not in `Backlog`, then it MUST have title, assignee, priority, estimate, iteration, and at least one label.
- An issue body SHOULD NOT be blank.

## Pull request rules

- A PR title MUST follow [Conventional Commits v1.0.0](https://www.conventionalcommits.org/en/v1.0.0/) standard.
- A PR body MUST NOT be blank.
- A PR body MUST have the next line `Closes #PR-NUMBER` for automatic issue linkage.
  
  > e.g. `Closes #23`
- A PR MUST be linked to a project.

## Code formatting rules

- A repository MUST have a formatting style defined in a file.
- A repository MUST have a readme that describes how to set up linter and formatter locally using a style defined in the file.

## Additional Code Conventions

- **Indenting:** 4 spaces MUST be used.
- **Descriptive Names:** Use descriptive names for functions or classes.
- **Comments:** Avoid comments in the code; aim for self-explanatory code.
- **Language Conventions:** Follow language code conventions style.
- **KISS Principle:** Always try to Keep It Simple (KISS).
- **DRY Principle:** Don't Repeat Yourself (DRY) when you have more than 3 repeats.
- **Library Usage:** Do not write a new version; search if it already exists and learn how to use it (we don't need another JS JSON library).
- **Testing Guidelines:** Include guidelines for writing tests. Specify whether tests are required for all new features and bug fixes.
- **Documentation:** Emphasize the importance of good documentation. Every repository, module, class, and method should have clear and concise documentation.
- **Code Review:** Define a process for code reviews. Specify who should review the code, and set expectations for feedback and response times.
- **Versioning:** Provide guidelines for versioning your software. Specify when to bump major, minor, or patch versions and how to update the version in your code.
- **Dependencies:** Specify guidelines for managing dependencies. Clearly state how to add, update, or remove dependencies and whether there are any restrictions on using specific libraries.
- **Security Practices:** Include guidelines for handling sensitive information and security best practices.
- **Naming Conventions:** Extend naming conventions to cover variables, constants, and file names. Consistent and meaningful names improve code readability.
- **Error Handling:** Provide guidelines for error handling, logging, and reporting. Define how to handle exceptions and errors to ensure a consistent approach.
- **Code Ownership:** Clarify the concept of code ownership. Specify who is responsible for maintaining different parts of the codebase.
- **Continuous Integration (CI) and Continuous Deployment (CD):** Outline CI/CD practices, including automated testing, deployment pipelines, and versioning strategies.
- **Accessibility and Internationalization:** If applicable, include guidelines for making your software accessible and supporting internationalization (i18n) and localization (l10n).
- **Performance:** Address performance considerations. Provide guidance on optimizing code and using profiling tools.
- **Community Guidelines:** If your project involves an open-source community, include guidelines for community contributions, issue reporting, and code of conduct.
