

- PackageDescription
- Package
- 
  - Package
- Package.Dependency
- Package.Dependency.Requirement
-  exact(\_:) Deprecated

Type Method

# exact(\_:)

Returns a requirement for the given exact version.

SwiftPMDeprecated

``` source
static func exact(_ version: Version) -> Package.Dependency.Requirement
```

## Parameters 

`version`  

The exact version of the dependency for this requirement.

## Discussion

Specifying exact version requirements are not recommended as they can cause conflicts in your dependency graph when multiple other packages depend on a package. As Swift packages follow the semantic versioning convention, think about specifying a version range instead.

The following example defines a version requirement that requires version 1.2.3 of a package.

```
.exact(“1.2.3”)
```

