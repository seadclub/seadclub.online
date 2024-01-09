+++
author = "github.com/btwkenji"
title = "Versioning Conventions"
date = "2023-12-27"
description = ""
tags = [
    "text",
    "docs",
    "help",
    "guide"
]
+++

## Introduction

This document outlines the versioning conventions adopted by the Software Engineering and Development Club at the State University of Information and Communication Technologies. These conventions are based on the standard versioning practices in the Rust programming language.

## Semantic Versioning (SemVer)

In alignment with Rust best practices, we follow Semantic Versioning (SemVer) for our software projects. SemVer consists of three components: MAJOR.MINOR.PATCH, indicating major, minor, and patch version releases.

1. **MAJOR version**: Increased for incompatible API changes.

2. **MINOR version**: Incremented for backward-compatible additions.

3. **PATCH version**: Incremented for backward-compatible bug fixes.

## Examples

### MAJOR Version Increment

```rust
// Before breaking change
pub const VERSION: &str = "1.0.0";

// After breaking change
pub const VERSION: &str = "2.0.0";
```

### MINOR Version Increment

```rust
// Before new feature addition
pub const VERSION: &str = "1.2.0";

// After adding a new feature
pub const VERSION: &str = "1.3.0";
```

### PATCH Version Increment

```rust
// Before bug fix
pub const VERSION: &str = "1.2.3";

// After fixing a bug
pub const VERSION: &str = "1.2.4";
```

### Pre-release Version

```rust
// Before stable release
pub const VERSION: &str = "1.2.3-alpha.1";
```

### Build Metadata

```rust
// With build metadata
pub const VERSION: &str = "1.2.3+20130313144700";
```

By following these versioning conventions, we aim to maintain clear communication about changes in our projects and enable seamless collaboration within our development community.
