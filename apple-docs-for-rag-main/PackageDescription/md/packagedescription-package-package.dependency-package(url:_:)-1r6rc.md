

- PackageDescription
- Package
- Package.Dependency
-  package(url:\_:) 

Type Method

# package(url:\_:)

Adds a package dependency starting with a specific minimum version, going up to and including a specific maximum version.

``` source
static func package(
    url: String,
    _ range: ClosedRange
) -> Package.Dependency
```

## Parameters 

`url`  

The valid Git URL of the package.

`range`  

The closed version range requirement.

## Return Value

A `Package.Dependency` instance.

## Discussion

The following example allows the Swift Package Manager to pick versions 1.2.3, 1.2.4, 1.2.5, as well as 1.2.6.

```
.package(url: "https://example.com/example-package.git", "1.2.3"..."1.2.6"),
```

## See Also

### Creating a Package Dependency

static func package(name: String, path: String) -> Package.Dependency

Adds a dependency to a package located at the given path on the filesystem.

static func package(url: String, from: Version) -> Package.Dependency

Adds a package dependency that uses the version requirement, starting with the given minimum version, going up to the next major version.

static func package(url: String, Range&lt;Version>) -> Package.Dependency

Adds a package dependency starting with a specific minimum version, up to but not including a specified maximum version.

static func package(url: String, branch: String) -> Package.Dependency

Adds a remote package dependency given a branch requirement.

static func package(url: String, revision: String) -> Package.Dependency

Adds a remote package dependency given a revision requirement.

static func package(url: String, exact: Version) -> Package.Dependency

Adds a package dependency that uses the exact version requirement.

static func package(path: String) -> Package.Dependency

Adds a dependency to a package located at the given path.

