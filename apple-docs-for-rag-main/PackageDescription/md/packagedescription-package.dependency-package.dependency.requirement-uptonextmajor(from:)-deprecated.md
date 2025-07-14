

- PackageDescription
- Package
- 
  - Package
- Package.Dependency
- Package.Dependency.Requirement
-  upToNextMajor(from:) Deprecated

Type Method

# upToNextMajor(from:)

A source control requirement bounded to the given version’s major version number.

SwiftPMDeprecated

``` source
static func upToNextMajor(from version: Version) -> Package.Dependency.Requirement
```

## Parameters 

`version`  

The minimum version for the version range.

## Return Value

A source control requirement instance.

## Discussion

Returns a requirement for a version range, starting at the given minimum version and going up to but not including the next major version. This is the recommended version requirement.

