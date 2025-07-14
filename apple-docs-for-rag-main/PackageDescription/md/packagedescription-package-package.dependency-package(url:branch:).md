

- PackageDescription
- Package
- Package.Dependency
-  package(url:branch:) 

Type Method

# package(url:branch:)

Adds a remote package dependency given a branch requirement.

SwiftPM 5.5+

``` source
static func package(
    url: String,
    branch: String
) -> Package.Dependency
```

## Parameters 

`url`  

The valid Git URL of the package.

`branch`  

A dependency requirement. See static methods on Package.Dependency.Requirement for available options.

## Return Value

A `Package.Dependency` instance.

## Discussion

```
.package(url: "https://example.com/example-package.git", branch: "main"),
```

## See Also

### Creating a Package Dependency

static func package(name: String, path: String) -> Package.Dependency

Adds a dependency to a package located at the given path on the filesystem.

static func package(url: String, from: Version) -> Package.Dependency

Adds a package dependency that uses the version requirement, starting with the given minimum version, going up to the next major version.

static func package(url: String, Range&lt;Version>) -> Package.Dependency

Adds a package dependency starting with a specific minimum version, up to but not including a specified maximum version.

static func package(url: String, ClosedRange&lt;Version>) -> Package.Dependency

Adds a package dependency starting with a specific minimum version, going up to and including a specific maximum version.

static func package(url: String, revision: String) -> Package.Dependency

Adds a remote package dependency given a revision requirement.

static func package(url: String, exact: Version) -> Package.Dependency

Adds a package dependency that uses the exact version requirement.

static func package(path: String) -> Package.Dependency

Adds a dependency to a package located at the given path.

