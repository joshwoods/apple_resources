

- PackageDescription
- Package
- Package.Dependency
-  package(url:branch:traits:) 

Type Method

# package(url:branch:traits:)

Adds a remote package dependency given a branch requirement.

SwiftPM 6.1+

``` source
static func package(
    url: String,
    branch: String,
    traits: Set = [.defaults]
) -> Package.Dependency
```

## Parameters 

`url`  

The valid Git URL of the package.

`branch`  

A dependency requirement. See static methods on Package.Dependency.Requirement for available options.

`traits`  

The trait configuration of this dependency. Defaults to enabling the default traits.

## Return Value

A `Package.Dependency` instance.

## Discussion

```
.package(url: "https://example.com/example-package.git", branch: "main"),
```

