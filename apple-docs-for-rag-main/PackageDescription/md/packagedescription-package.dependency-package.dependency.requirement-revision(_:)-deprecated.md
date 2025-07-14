

- PackageDescription
- Package
- 
  - Package
- Package.Dependency
- Package.Dependency.Requirement
-  revision(\_:) Deprecated

Type Method

# revision(\_:)

Returns a requirement for a source control revision such as the hash of a commit.

SwiftPMDeprecated

``` source
static func revision(_ ref: String) -> Package.Dependency.Requirement
```

## Parameters 

`ref`  

The Git revision, usually a commit hash.

## Discussion

Note that packages that use commit-based dependency requirements can’t be depended upon by packages that use version-based dependency requirements; you should remove commit-based dependency requirements before publishing a version of your package.

The following example defines a version requirement for a specific commit hash.

```
.revision(“e74b07278b926c9ec6f9643455ea00d1ce04a021”)
```

