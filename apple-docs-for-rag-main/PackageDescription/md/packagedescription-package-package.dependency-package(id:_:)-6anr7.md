

- PackageDescription
- Package
- Package.Dependency
-  package(id:\_:) 

Type Method

# package(id:\_:)

Adds a package dependency starting with a specific minimum version, going up to and including a specific maximum version.

SwiftPM 5.7+

``` source
static func package(
    id: String,
    _ range: ClosedRange
) -> Package.Dependency
```

## Parameters 

`id`  

The identity of the package.

`range`  

The closed version range requirement.

## Return Value

A `Package.Dependency` instance.

## Discussion

The following example allows the Swift Package Manager to pick versions 1.2.3, 1.2.4, 1.2.5, as well as 1.2.6.

```
.package(id: "scope.name", "1.2.3"..."1.2.6"),
```

