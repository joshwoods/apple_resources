

- PackageDescription
- Package
- Package.Dependency
-  package(id:exact:) 

Type Method

# package(id:exact:)

Adds a package dependency that uses the exact version requirement.

SwiftPM 5.7+

``` source
static func package(
    id: String,
    exact version: Version
) -> Package.Dependency
```

## Parameters 

`id`  

The identity of the package.

`version`  

The exact version of the dependency for this requirement.

## Return Value

A `Package.Dependency` instance.

## Discussion

Specifying exact version requirements are not recommended as they can cause conflicts in your dependency graph when multiple other packages depend on a package. Because Swift packages follow the semantic versioning convention, think about specifying a version range instead.

The following example instructs the Swift Package Manager to use version `1.2.3`.

```
.package(id: "scope.name", exact: "1.2.3"),
```

