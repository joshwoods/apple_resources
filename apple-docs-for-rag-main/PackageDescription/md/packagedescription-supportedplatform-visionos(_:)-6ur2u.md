

- PackageDescription
- SupportedPlatform
-  visionOS(\_:) 

Type Method

# visionOS(\_:)

Configure the minimum deployment target version for the visionOS platform using a custom version string.

SwiftPM 5.9+

``` source
static func visionOS(_ versionString: String) -> SupportedPlatform
```

## Parameters 

`versionString`  

The minimum deployment target as a string representation of two or three dot-separated integers, such as `1.0.0`.

## Return Value

A `SupportedPlatform` instance.

## Discussion

The version string must be a series of two or three dot-separated integers, such as `1.0` or `1.0.0`.

Since

First available in PackageDescription 5.9

## See Also

### Supporting visionOS

static func visionOS(SupportedPlatform.VisionOSVersion) -> SupportedPlatform

Configure the minimum deployment target version for the visionOS platform.

static let visionOS: Platform

The visionOS platform.

struct VisionOSVersion

The supported visionOS version.

