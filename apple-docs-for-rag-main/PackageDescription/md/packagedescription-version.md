

- PackageDescription
-  Version 

Structure

# Version

A version according to the semantic versioning specification.

``` source
struct Version
```

## Overview

A package version consists of three integers separated by periods, for example `1.0.0`. It must conform to the semantic versioning standard in order to ensure that your package behaves in a predictable manner once developers update their package dependency to a newer version. To achieve predictability, the semantic versioning specification proposes a set of rules and requirements that dictate how version numbers are assigned and incremented. To learn more about the semantic versioning specification, visit Semantic Versioning 2.0.0.

The major version  
The first digit of a version, or *major version*, signifies breaking changes to the API that require updates to existing clients. For example, the semantic versioning specification considers renaming an existing type, removing a method, or changing a method’s signature breaking changes. This also includes any backward-incompatible bug fixes or behavioral changes of the existing API.

The minor version  
Update the second digit of a version, or *minor version*, if you add functionality in a backward-compatible manner. For example, the semantic versioning specification considers adding a new method or type without changing any other API to be backward-compatible.

The patch version  
Increase the third digit of a version, or *patch version*, if you’re making a backward-compatible bug fix. This allows clients to benefit from bugfixes to your package without incurring any maintenance burden.

## Topics

### Initializers

init(Int, Int, Int, prereleaseIdentifiers: [String], buildMetadataIdentifiers: [String])

Initializes a version struct with the provided components of a semantic version.

### Instance Properties

let buildMetadataIdentifiers: [String]

The build metadata of this version according to the semantic versioning standard, such as a commit hash.

let major: Int

The major version according to the semantic versioning standard.

let minor: Int

The minor version according to the semantic versioning standard.

let patch: Int

The patch version according to the semantic versioning standard.

let prereleaseIdentifiers: [String]

The pre-release identifier according to the semantic versioning standard, such as `-beta.1`.

### Default Implementations

Comparable Implementations

CustomStringConvertible Implementations

Equatable Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringLiteral Implementations

ExpressibleByUnicodeScalarLiteral Implementations

LosslessStringConvertible Implementations

## Relationships

### Conforms To

- Comparable
- Copyable
- CustomStringConvertible
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- LosslessStringConvertible
- Sendable

## See Also

### Describing a Package Dependency

let kind: Package.Dependency.Kind

A description of the package dependency.

