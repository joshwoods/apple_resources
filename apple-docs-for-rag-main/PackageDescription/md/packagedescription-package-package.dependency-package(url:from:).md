

- PackageDescription
- Package
- Package.Dependency
-  package(url:from:) 

Type Method

# package(url:from:)

Adds a package dependency that uses the version requirement, starting with the given minimum version, going up to the next major version.

``` source
static func package(
    url: String,
    from version: Version
) -> Package.Dependency
```

## Parameters 

`url`  

The valid Git URL of the package.

`version`  

The minimum version requirement.

## Return Value

A `Package.Dependency` instance.

## Discussion

This is the recommended way to specify a remote package dependency. It allows you to specify the minimum version you require, allows updates that include bug fixes and backward-compatible feature updates, but requires you to explicitly update to a new major version of the dependency. This approach provides the maximum flexibility on which version to use, while making sure you don’t update to a version with breaking changes, and helps to prevent conflicts in your dependency graph.

The following example allows the Swift Package Manager to select a version like a `1.2.3`, `1.2.4`, or `1.3.0`, but not `2.0.0`.

```
.package(url: "https://example.com/example-package.git", from: "1.2.3"),
```

## See Also

### Creating a Package Dependency

static func package(name: String, path: String) -> Package.Dependency

Adds a dependency to a package located at the given path on the filesystem.

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

