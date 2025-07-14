

- PackageDescription
- Package
- Package.Dependency
-  package(id:\_:) 

Type Method

# package(id:\_:)

Adds a package dependency starting with a specific minimum version, up to but not including a specified maximum version.

SwiftPM 5.7+

``` source
static func package(
    id: String,
    _ range: Range
) -> Package.Dependency
```

## Parameters 

`id`  

The identity of the package.

`range`  

The custom version range requirement.

## Return Value

A `Package.Dependency` instance.

## Discussion

The following example allows the Swift Package Manager to pick versions `1.2.3`, `1.2.4`, `1.2.5`, but not `1.2.6`.

```
.package(id: "scope.name", "1.2.3"..

The following example allows the Swift Package Manager to pick versions between 1.0.0 and 2.0.0

```
.package(id: "scope.name", .upToNextMajor(from: "1.0.0"),
```

The following example allows the Swift Package Manager to pick versions between 1.0.0 and 1.1.0

```
.package(id: "scope.name", .upToNextMinor(from: "1.0.0"),
```

