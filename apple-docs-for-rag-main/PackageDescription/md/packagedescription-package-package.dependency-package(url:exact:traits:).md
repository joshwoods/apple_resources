

- PackageDescription
- Package
- Package.Dependency
-  package(url:exact:traits:) 

Type Method

# package(url:exact:traits:)

Adds a package dependency that uses the exact version requirement.

SwiftPM 6.1+

``` source
static func package(
    url: String,
    exact version: Version,
    traits: Set = [.defaults]
) -> Package.Dependency
```

## Parameters 

`url`  

The valid Git URL of the package.

`version`  

The exact version of the dependency for this requirement.

`traits`  

The trait configuration of this dependency. Defaults to enabling the default traits.

## Return Value

A `Package.Dependency` instance.

## Discussion

Specifying exact version requirements are not recommended as they can cause conflicts in your dependency graph when other packages depend on this package. As Swift packages follow the semantic versioning convention, think about specifying a version range instead.

The following example instructs the Swift Package Manager to use version `1.2.3`.

```
.package(url: "https://example.com/example-package.git", exact: "1.2.3"),
```

