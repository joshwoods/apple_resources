

- PackageDescription
- Package
- Package.Dependency
-  Package.Dependency.Kind 

Enumeration

# Package.Dependency.Kind

The type of dependency.

SwiftPM 5.6+

``` source
enum Kind
```

## Topics

### Enumeration Cases

case fileSystem(name: String?, path: String)

A dependency located at the given path.

case registry(id: String, requirement: Package.Dependency.RegistryRequirement)

A dependency based on a registry requirement.

case sourceControl(name: String?, location: String, requirement: Package.Dependency.SourceControlRequirement)

A dependency based on a source control requirement.

