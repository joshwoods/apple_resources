

- PackageDescription
- Package
- Package.Dependency
-  package(url:exact:) 

Type Method

# package(url:exact:)

Adds a package dependency that uses the exact version requirement.

SwiftPM 5.6+

``` source
static func package(
    url: String,
    exact version: Version
) -> Package.Dependency
```

## Parameters 

`url`  

The valid Git URL of the package.

`version`  

The exact version of the dependency for this requirement.

## Return Value

A `Package.Dependency` instance.

## Discussion

Specifying exact version requirements are not recommended as they can cause conflicts in your dependency graph when other packages depend on this package. As Swift packages follow the semantic versioning convention, think about specifying a version range instead.

The following example instructs the Swift Package Manager to use version `1.2.3`.

```
.package(url: "https://example.com/example-package.git", exact: "1.2.3"),
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

static func package(url: String, branch: String) -> Package.Dependency

Adds a remote package dependency given a branch requirement.

static func package(url: String, revision: String) -> Package.Dependency

Adds a remote package dependency given a revision requirement.

static func package(path: String) -> Package.Dependency

Adds a dependency to a package located at the given path.

