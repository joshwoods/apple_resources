

- PackageDescription
- Package
- 
  - Package
- Package.Dependency
- Package.Dependency.Requirement
-  branch(\_:) Deprecated

Type Method

# branch(\_:)

Returns a requirement for a source control branch.

SwiftPMDeprecated

``` source
static func branch(_ name: String) -> Package.Dependency.Requirement
```

## Parameters 

`name`  

The name of the branch.

## Discussion

Note that packages that use branch-based dependency requirements can’t be depended upon by packages that use version-based dependency requirements; you should remove branch-based dependency requirements before publishing a version of your package.

The following example defines a version requirement that accepts any change in the develop branch.

```
.branch(“develop”)
```

