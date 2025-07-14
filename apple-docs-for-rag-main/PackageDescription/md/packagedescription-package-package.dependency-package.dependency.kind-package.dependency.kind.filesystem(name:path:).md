

- PackageDescription
- Package
- Package.Dependency
- Package.Dependency.Kind
-  Package.Dependency.Kind.fileSystem(name:path:) 

Case

# Package.Dependency.Kind.fileSystem(name:path:)

A dependency located at the given path.

SwiftPM 5.6+

``` source
case fileSystem(
    name: String?,
    path: String
)
```

## Parameters 

`name`  

The name of the dependency.

`path`  

The path to the dependency.

