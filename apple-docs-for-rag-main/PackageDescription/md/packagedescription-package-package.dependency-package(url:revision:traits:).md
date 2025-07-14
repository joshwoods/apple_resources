

- PackageDescription
- Package
- Package.Dependency
-  package(url:revision:traits:) 

Type Method

# package(url:revision:traits:)

Adds a remote package dependency given a revision requirement.

SwiftPM 6.1+

``` source
static func package(
    url: String,
    revision: String,
    traits: Set = [.defaults]
) -> Package.Dependency
```

## Parameters 

`url`  

The valid Git URL of the package.

`revision`  

A dependency requirement. See static methods on Package.Dependency.Requirement for available options.

`traits`  

The trait configuration of this dependency. Defaults to enabling the default traits.

## Return Value

A `Package.Dependency` instance.

## Discussion

```
.package(url: "https://example.com/example-package.git", revision: "aa681bd6c61e22df0fd808044a886fc4a7ed3a65"),
```

