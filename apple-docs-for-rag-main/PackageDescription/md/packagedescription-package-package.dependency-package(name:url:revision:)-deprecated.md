

- PackageDescription
- Package
- Package.Dependency
-  package(name:url:revision:) Deprecated

Type Method

# package(name:url:revision:)

Adds a remote package dependency given a revision requirement.

SwiftPM 5.5–5.6Deprecated

``` source
static func package(
    name: String,
    url: String,
    revision: String
) -> Package.Dependency
```

Deprecated

use package(url:revision:) instead

## Parameters 

`name`  

The name of the package, or nil to deduce it from the URL.

`url`  

The valid Git URL of the package.

`revision`  

A dependency requirement. See static methods on Package.Dependency.Requirement for available options.

## Return Value

A `Package.Dependency` instance.

## Discussion

```
.package(url: "https://example.com/example-package.git", revision: "aa681bd6c61e22df0fd808044a886fc4a7ed3a65"),
```

