

- PackageDescription
- SupportedPlatform
-  visionOS(\_:) 

Type Method

# visionOS(\_:)

Configure the minimum deployment target version for the visionOS platform.

SwiftPM 5.9+

``` source
static func visionOS(_ version: SupportedPlatform.VisionOSVersion) -> SupportedPlatform
```

## Parameters 

`version`  

The minimum deployment target that the package supports.

## Return Value

A `SupportedPlatform` instance.

## Discussion

Since

First available in PackageDescription 5.9

## See Also

### Supporting visionOS

static func visionOS(String) -> SupportedPlatform

Configure the minimum deployment target version for the visionOS platform using a custom version string.

static let visionOS: Platform

The visionOS platform.

struct VisionOSVersion

The supported visionOS version.

