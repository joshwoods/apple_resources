

- PackageDescription
- Package
- Package.Dependency
-  Package.Dependency.RegistryRequirement 

Enumeration

# Package.Dependency.RegistryRequirement

An enum that represents the requirement for a package dependency.

SwiftPM 999.0+

``` source
enum RegistryRequirement
```

## Overview

Decide whether your project accepts updates to a package dependency up to the next major version or up to the next minor version. To be more restrictive, select a specific version range or an exact version. Major versions tend to have more significant changes than minor versions, and may require you to modify your code when they update. The version rule requires Swift packages to conform to semantic versioning. To learn more about the semantic versioning standard, visit the Semantic Versioning 2.0.0 website.

## Topics

### Enumeration Cases

case exact(Version)

A requirement based on an exact version.

case range(Range&lt;Version>)

A requirement based on a range of versions.

