

- PackageDescription
- Package
- Package.Dependency
-  package(name:path:) 

Type Method

# package(name:path:)

Adds a dependency to a package located at the given path on the filesystem.

SwiftPM 5.2+

``` source
static func package(
    name: String,
    path: String
) -> Package.Dependency
```

## Parameters 

`name`  

The name of the Swift package.

`path`  

The file system path to the package.

## Return Value

A package dependency.

## Discussion

Swift Package Manager uses the package dependency as-is and doesn’t perform any source control access. Local package dependencies are especially useful during development of a new package or when working on multiple tightly coupled packages.

## See Also

### Creating a Package Dependency

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

