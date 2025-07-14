

- PackageDescription
- Package
- Package.Dependency
-  package(url:\_:) Deprecated

Type Method

# package(url:\_:)

Adds a remote package dependency given a version requirement.

SwiftPMDeprecated

``` source
static func package(
    url: String,
    _ requirement: Package.Dependency.Requirement
) -> Package.Dependency
```

Deprecated

use specific requirement APIs instead (e.g. use 'branch:' instead of '.branch')

## Parameters 

`url`  

The valid Git URL of the package.

`requirement`  

A dependency requirement. See static methods on `Package.Dependency.Requirement` for available options.

## Return Value

A `Package.Dependency` instance.

