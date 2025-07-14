

- PackageDescription
- Package
- Package.Dependency
-  package(name:path:traits:) 

Type Method

# package(name:path:traits:)

Adds a dependency to a package located at the given path on the filesystem.

SwiftPM 6.1+

``` source
static func package(
    name: String,
    path: String,
    traits: Set = [.defaults]
) -> Package.Dependency
```

## Parameters 

`name`  

The name of the Swift package.

`path`  

The file system path to the package.

`traits`  

The trait configuration of this dependency. Defaults to enabling the default traits.

## Return Value

A package dependency.

## Discussion

Swift Package Manager uses the package dependency as-is and doesn’t perform any source control access. Local package dependencies are especially useful during development of a new package or when working on multiple tightly coupled packages.

