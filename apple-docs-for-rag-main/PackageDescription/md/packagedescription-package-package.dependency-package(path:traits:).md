

- PackageDescription
- Package
- Package.Dependency
-  package(path:traits:) 

Type Method

# package(path:traits:)

Adds a dependency to a package located at the given path.

SwiftPM 6.1+

``` source
static func package(
    path: String,
    traits: Set = [.defaults]
) -> Package.Dependency
```

## Parameters 

`path`  

The file system path to the package.

`traits`  

The trait configuration of this dependency. Defaults to enabling the default traits.

## Return Value

A package dependency.

## Discussion

The Swift Package Manager uses the package dependency as-is and does not perform any source control access. Local package dependencies are especially useful during development of a new package or when working on multiple tightly coupled packages.

