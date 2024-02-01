+++
author = "github.com/btwkenji"
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

<!--toc:start-->
- [Priority values](#priority-values)
- [Estimation values](#estimation-values)
- [Repository rules](#repository-rules)
- [Branch rules](#branch-rules)
- [Commits](#commits)
- [Issue rules](#issue-rules)
- [Pull request rules](#pull-request-rules)
- [Code formatting rules](#code-formatting-rules)
- [Additional Code Conventions](#additional-code-conventions)
<!--toc:end-->

> The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](https://www.rfc-editor.org/rfc/rfc2119)

## Priority values

- `Low` - low priority (small pinpoint improvements).

- `Normal` - normal priority (main features, fixes).
 
- `High` - high priority (more important main feature, fix).

- `Blocker` - other tasks can't be performed until this issue is resolved.

## Estimation values

- `Hours` - an issue might take 1-8 hours.
 
- `Days` - an issue might take 1-7 days.
 
- `Weeks` - an issue might take 1-2 weeks.

If estimation exceeds 2 weeks, an issue MUST be split into smaller ones.

## Repository rules

- A repository MUST allow either `merge commits` or `rebase merging`.

- A repository MUST NOT allow `squash merging`.

## Branch rules

- A main branch name MUST be `master`.
 
- A master branch name MUST be protected.
 
- A master branch name MUST NOT be force pushed.
 
- A new branch MUST be created for each issue or feature.
 
- A new branch name MUST follow the next pattern `<type>/PR-NUMBER/optional-info`, where `<type>` is from [Conventional Commits v1.0.0](https://www.conventionalcommits.org/en/v1.0.0/) standard.

e.g.

> `fix/#9`

> `feat/#883/hatsune-miku-the-real-one`

> `docs/#1/me-and-waifu`

## Commits

- A commit message MUST follow [Conventional Commits v1.0.0](https://www.conventionalcommits.org/en/v1.0.0/) standard.

- A commit message MUST contain the pull request number (e.g., #54) in a scope.
  
  > e.g. `fix(#53): change button color to red`
- A commit SHOULD be signed off.

## Issue rules

- If an issue is not in `Backlog`, then it MUST have title, description, priority, estimate and at least one label.

- An issue body SHOULD NOT be blank.

## Pull request rules

- A PR title MUST follow [Conventional Commits v1.0.0](https://www.conventionalcommits.org/en/v1.0.0/) standard.

- A PR body MUST NOT be blank.
  
- A PR MUST be linked to a project.

## Code formatting rules

- A repository MUST have a formatting style defined in a project.

- A repository MUST have a README that describes how to set up linter and formatter locally using a style defined in the file (If there are any specifics set up challenges).

## Additional Code Conventions

**Indenting:** 4 spaces MUST be used.

**Descriptive Names:** Use descriptive names for functions or classes.

**Comments:** Avoid comments in the code; aim for self-explanatory code.

**Language Conventions:** Follow language code conventions style.

**KISS Principle:** Always try to Keep It Simple (KISS).

**DRY Principle:** Don't Repeat Yourself (DRY) when you have more than 3 repeats.

**Library Usage:** Do not write a new version; search if it already exists and learn how to use it (we don't need another JS JSON library).

**Testing:** It always nice when a project has some unit tests, or other types of tests. So atleast unit tests are required, and MUST cover as many as possible.

**Documentation:** Emphasize the importance of good documentation. Every repository, module, class, and method should have clear and concise documented.

**Versioning:** In alignment with best practices, we follow [Semantic Versioning (SemVer)](/docs/versioning-conventions) for our software projects.

**Code Ownership:** Always clarify the concept of code ownership. Know for what part you are responsible to. Specify who is responsible for maintaining different parts of the codebase.

**Continuous Integration (CI) and Continuous Deployment (CD):** Outline CI/CD practices, including automated testing, deployment pipelines, and versioning strategies. Always try to automate.

**Accessibility and Internationalization:** If applicable, include guidelines for making your software accessible and supporting internationalization (i18n) and localization (l10n).

**Community Guidelines:** If your project involves an open-source community, include guidelines for community contributions, issue reporting, and code of conduct.
