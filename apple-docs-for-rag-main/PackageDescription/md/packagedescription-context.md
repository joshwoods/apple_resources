

- PackageDescription
-  Context 

Structure

# Context

The context information for a Swift package.

SwiftPM 5.6+

``` source
struct Context
```

## Overview

The context encapsulates states that are known when Swift Package Manager interprets the package manifest, for example the location in the file system where the current package resides.

## Topics

### Type Properties

static var environment: [String : String]

Snapshot of the system environment variables.

static var gitInformation: GitInformation?

Information about the git status of a given package, if available.

static var packageDirectory: String

The directory that contains `Package.swift`.

## Relationships

### Conforms To

- Sendable

## See Also

### Creating a Package

class Package

The configuration of a Swift package.

