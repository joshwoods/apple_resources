

- PackageDescription
- Package
- Package.Dependency
-  package(name:url:\_:) Deprecated

Type Method

# package(name:url:\_:)

Adds a package dependency starting with a specific minimum version, up to but not including a specified maximum version.

SwiftPM 5.2–5.6Deprecated

``` source
static func package(
    name: String,
    url: String,
    _ range: Range
) -> Package.Dependency
```

Deprecated

use package(url:\_:) instead

## Parameters 

`name`  

The name of the package, or `nil` to deduce it from the URL.

`url`  

The valid Git URL of the package.

`range`  

The custom version range requirement.

## Return Value

A `Package.Dependency` instance.

## Discussion

The following example allows the Swift Package Manager to pick versions `1.2.3`, `1.2.4`, `1.2.5`, but not `1.2.6`.

```
.package(url: "https://example.com/example-package.git", "1.2.3"..

