

- PackageDescription
- Package
- Package.Dependency
-  package(url:\_:traits:) 

Type Method

# package(url:\_:traits:)

Adds a package dependency starting with a specific minimum version, going up to and including a specific maximum version.

SwiftPM 6.1+

``` source
static func package(
    url: String,
    _ range: ClosedRange,
    traits: Set = [.defaults]
) -> Package.Dependency
```

## Parameters 

`url`  

The valid Git URL of the package.

`range`  

The closed version range requirement.

`traits`  

The trait configuration of this dependency. Defaults to enabling the default traits.

## Return Value

A `Package.Dependency` instance.

## Discussion

The following example allows the Swift Package Manager to pick versions 1.2.3, 1.2.4, 1.2.5, as well as 1.2.6.

```
.package(url: "https://example.com/example-package.git", "1.2.3"..."1.2.6"),
```

