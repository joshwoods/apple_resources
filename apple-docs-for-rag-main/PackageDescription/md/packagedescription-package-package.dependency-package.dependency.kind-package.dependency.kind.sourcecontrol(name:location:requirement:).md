

- PackageDescription
- Package
- Package.Dependency
- Package.Dependency.Kind
-  Package.Dependency.Kind.sourceControl(name:location:requirement:) 

Case

# Package.Dependency.Kind.sourceControl(name:location:requirement:)

A dependency based on a source control requirement.

SwiftPM 5.6+

``` source
case sourceControl(
    name: String?,
    location: String,
    requirement: Package.Dependency.SourceControlRequirement
)
```

## Parameters 

`name`  

The name of the dependency.

`location`  

The Git URL of the dependency.

`requirement`  

The version-based requirement for a package.

