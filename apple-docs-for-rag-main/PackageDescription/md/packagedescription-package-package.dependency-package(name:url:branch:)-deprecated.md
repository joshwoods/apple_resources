

- PackageDescription
- Package
- Package.Dependency
-  package(name:url:branch:) Deprecated

Type Method

# package(name:url:branch:)

Adds a remote package dependency given a branch requirement.

SwiftPM 5.5–5.6Deprecated

``` source
static func package(
    name: String,
    url: String,
    branch: String
) -> Package.Dependency
```

Deprecated

use package(url:branch:) instead

## Parameters 

`name`  

The name of the package, or nil to deduce it from the URL.

`url`  

The valid Git URL of the package.

`branch`  

A dependency requirement. See static methods on Package.Dependency.Requirement for available options.

## Return Value

A `Package.Dependency` instance.

## Discussion

```
.package(url: "https://example.com/example-package.git", branch: "main"),
```

