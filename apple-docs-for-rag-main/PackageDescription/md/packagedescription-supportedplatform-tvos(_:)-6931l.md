

- PackageDescription
- SupportedPlatform
-  tvOS(\_:) 

Type Method

# tvOS(\_:)

Configures the minimum deployment target version for the tvOS platform.

``` source
static func tvOS(_ version: SupportedPlatform.TVOSVersion) -> SupportedPlatform
```

## Parameters 

`version`  

The minimum deployment target that the package supports.

## Return Value

A `SupportedPlatform` instance.

## Discussion

Since

First available in PackageDescription 5.0

## See Also

### Supporting tvOS

static func tvOS(String) -> SupportedPlatform

Configures the minimum deployment target version for the tvOS platform using a custom version string.

static let tvOS: Platform

The tvOS platform.

struct TVOSVersion

The supported tvOS version.

