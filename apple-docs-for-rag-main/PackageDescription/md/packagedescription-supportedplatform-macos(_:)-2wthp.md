

- PackageDescription
- SupportedPlatform
-  macOS(\_:) 

Type Method

# macOS(\_:)

Configures the minimum deployment target version for the macOS platform.

``` source
static func macOS(_ version: SupportedPlatform.MacOSVersion) -> SupportedPlatform
```

## Parameters 

`version`  

The minimum deployment target that the package supports.

## Discussion

Since

First available in PackageDescription 5.0

## See Also

### Supporting macOS

static func macOS(String) -> SupportedPlatform

Configures the minimum deployment target version for the macOS platform using a version string.

static let macOS: Platform

The macOS platform.

struct MacOSVersion

The supported macOS version.

