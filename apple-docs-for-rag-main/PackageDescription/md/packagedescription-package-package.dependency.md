

- PackageDescription
- Package
-  Package.Dependency 

Class

# Package.Dependency

A package dependency of a Swift package.

``` source
class Dependency
```

## Overview

A package dependency consists of a Git URL to the source of the package, and a requirement for the version of the package.

Swift Package Manager performs a process called *dependency resolution* to determine the exact version of the package dependencies that an app or other Swift package can use. The `Package.resolved` file records the results of the dependency resolution and lives in the top-level directory of a Swift package. If you add the Swift package as a package dependency to an app for an Apple platform, you can find the `Package.resolved` file inside your `.xcodeproj` or `.xcworkspace`.

## Topics

### Creating a Package Dependency

static func package(name: String, path: String) -> Package.Dependency

Adds a dependency to a package located at the given path on the filesystem.

static func package(url: String, from: Version) -> Package.Dependency

Adds a package dependency that uses the version requirement, starting with the given minimum version, going up to the next major version.

static func package(url: String, Range&lt;Version>) -> Package.Dependency

Adds a package dependency starting with a specific minimum version, up to but not including a specified maximum version.

static func package(url: String, ClosedRange&lt;Version>) -> Package.Dependency

Adds a package dependency starting with a specific minimum version, going up to and including a specific maximum version.

static func package(url: String, branch: String) -> Package.Dependency

Adds a remote package dependency given a branch requirement.

static func package(url: String, revision: String) -> Package.Dependency

Adds a remote package dependency given a revision requirement.

static func package(url: String, exact: Version) -> Package.Dependency

Adds a package dependency that uses the exact version requirement.

static func package(path: String) -> Package.Dependency

Adds a dependency to a package located at the given path.

### Declaring Requirements

var requirement: Package.Dependency.Requirement

The dependency requirement of the package dependency.

Deprecated

enum Requirement

An enum that represents the requirement for a package dependency.

Deprecated

### Describing a Package Dependency

let kind: Package.Dependency.Kind

A description of the package dependency.

struct Version

A version according to the semantic versioning specification.

### Structures

struct Trait

A struct representing an enabled trait of a dependency.

### Instance Properties

var name: String?

The name of the dependency.

Deprecated

let traits: Set&lt;Package.Dependency.Trait>

The dependencies traits configuration.

var url: String?

The Git URL of the package dependency.

Deprecated

### Type Methods

static func package(id: String, Range&lt;Version>) -> Package.Dependency

Adds a package dependency starting with a specific minimum version, up to but not including a specified maximum version.

static func package(id: String, ClosedRange&lt;Version>) -> Package.Dependency

Adds a package dependency starting with a specific minimum version, going up to and including a specific maximum version.

static func package(id: String, Range&lt;Version>, traits: Set&lt;Package.Dependency.Trait>) -> Package.Dependency

Adds a package dependency starting with a specific minimum version, up to but not including a specified maximum version.

static func package(id: String, ClosedRange&lt;Version>, traits: Set&lt;Package.Dependency.Trait>) -> Package.Dependency

Adds a package dependency starting with a specific minimum version, going up to and including a specific maximum version.

static func package(id: String, exact: Version) -> Package.Dependency

Adds a package dependency that uses the exact version requirement.

static func package(id: String, exact: Version, traits: Set&lt;Package.Dependency.Trait>) -> Package.Dependency

Adds a package dependency that uses the exact version requirement.

static func package(id: String, from: Version) -> Package.Dependency

Adds a package dependency that uses the version requirement, starting with the given minimum version, going up to the next major version.

static func package(id: String, from: Version, traits: Set&lt;Package.Dependency.Trait>) -> Package.Dependency

Adds a package dependency that uses the version requirement, starting with the given minimum version, going up to the next major version.

static func package(name: String, path: String, traits: Set&lt;Package.Dependency.Trait>) -> Package.Dependency

Adds a dependency to a package located at the given path on the filesystem.

static func package(name: String?, url: String, Package.Dependency.Requirement) -> Package.Dependency

Adds a remote package dependency with a given version requirement.

Deprecated

static func package(name: String, url: String, ClosedRange&lt;Version>) -> Package.Dependency

Adds a package dependency starting with a specific minimum version, going up to and including a specific maximum version.

Deprecated

static func package(name: String, url: String, Range&lt;Version>) -> Package.Dependency

Adds a package dependency starting with a specific minimum version, up to but not including a specified maximum version.

Deprecated

static func package(name: String, url: String, branch: String) -> Package.Dependency

Adds a remote package dependency given a branch requirement.

Deprecated

static func package(name: String, url: String, from: Version) -> Package.Dependency

Adds a package dependency that uses the version requirement, starting with the given minimum version, going up to the next major version.

Deprecated

static func package(name: String, url: String, revision: String) -> Package.Dependency

Adds a remote package dependency given a revision requirement.

Deprecated

static func package(path: String, traits: Set&lt;Package.Dependency.Trait>) -> Package.Dependency

Adds a dependency to a package located at the given path.

static func package(url: String, Package.Dependency.Requirement) -> Package.Dependency

Adds a remote package dependency given a version requirement.

Deprecated

static func package(url: String, Range&lt;Version>, traits: Set&lt;Package.Dependency.Trait>) -> Package.Dependency

Adds a package dependency starting with a specific minimum version, up to but not including a specified maximum version.

static func package(url: String, ClosedRange&lt;Version>, traits: Set&lt;Package.Dependency.Trait>) -> Package.Dependency

Adds a package dependency starting with a specific minimum version, going up to and including a specific maximum version.

static func package(url: String, branch: String, traits: Set&lt;Package.Dependency.Trait>) -> Package.Dependency

Adds a remote package dependency given a branch requirement.

static func package(url: String, exact: Version, traits: Set&lt;Package.Dependency.Trait>) -> Package.Dependency

Adds a package dependency that uses the exact version requirement.

static func package(url: String, from: Version, traits: Set&lt;Package.Dependency.Trait>) -> Package.Dependency

Adds a package dependency that uses the version requirement, starting with the given minimum version, going up to the next major version.

static func package(url: String, revision: String, traits: Set&lt;Package.Dependency.Trait>) -> Package.Dependency

Adds a remote package dependency given a revision requirement.

### Enumerations

enum Kind

The type of dependency.

enum RegistryRequirement

An enum that represents the requirement for a package dependency.

enum SourceControlRequirement

An enum that represents the requirement for a package dependency.

## See Also

### Declaring Package Dependencies

var dependencies: [Package.Dependency]

The list of package dependencies.

