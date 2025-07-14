

- PackageDescription
- Package
- 
  - Package
- Package.Dependency
- Package.Dependency.Requirement
-  upToNextMinor(from:) Deprecated

Type Method

# upToNextMinor(from:)

A source control requirement bounded to the given version’s minor version number.

SwiftPMDeprecated

``` source
static func upToNextMinor(from version: Version) -> Package.Dependency.Requirement
```

## Parameters 

`version`  

The minimum version for the version range.

## Return Value

A source control requirement instance.

## Discussion

Returns a requirement for a version range, starting at the given minimum version and going up to but not including the next minor version.

