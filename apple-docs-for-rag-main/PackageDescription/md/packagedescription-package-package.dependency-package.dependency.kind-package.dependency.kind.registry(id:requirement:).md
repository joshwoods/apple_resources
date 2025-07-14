

- PackageDescription
- Package
- Package.Dependency
- Package.Dependency.Kind
-  Package.Dependency.Kind.registry(id:requirement:) 

Case

# Package.Dependency.Kind.registry(id:requirement:)

A dependency based on a registry requirement.

SwiftPM 5.6+

``` source
case registry(
    id: String,
    requirement: Package.Dependency.RegistryRequirement
)
```

## Parameters 

`id`  

The package identifier of the dependency.

`requirement`  

The version based requirement for a package.

