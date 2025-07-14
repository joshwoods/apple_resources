

- PackageDescription
- Package
- Package.Dependency
-  package(name:url:\_:) Deprecated

Type Method

# package(name:url:\_:)

Adds a remote package dependency with a given version requirement.

SwiftPM 5.2–5.6Deprecated

``` source
static func package(
    name: String?,
    url: String,
    _ requirement: Package.Dependency.Requirement
) -> Package.Dependency
```

Deprecated

use specific requirement APIs instead (e.g. use 'branch:' instead of '.branch')

## Parameters 

`name`  

The name of the Swift package or `nil` to deduce the name from the package’s Git URL.

`url`  

The valid Git URL of the package.

`requirement`  

A dependency requirement. See static methods on Package.Dependency.Requirement for available options.

## Return Value

A `Package.Dependency` instance.

