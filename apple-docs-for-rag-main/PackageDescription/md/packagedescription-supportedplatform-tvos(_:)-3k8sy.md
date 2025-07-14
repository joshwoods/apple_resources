

- PackageDescription
- SupportedPlatform
-  tvOS(\_:) 

Type Method

# tvOS(\_:)

Configures the minimum deployment target version for the tvOS platform using a custom version string.

``` source
static func tvOS(_ versionString: String) -> SupportedPlatform
```

## Parameters 

`versionString`  

The minimum deployment target as a string representation of two or three dot-separated integers, such as `9.0.1`.

## Return Value

A `SupportedPlatform` instance.

## Discussion

The version string must be a series of two or three dot-separated integers,such as `9.0` or `9.0.1`.

Since

First available in PackageDescription 5.0

## See Also

### Supporting tvOS

static func tvOS(SupportedPlatform.TVOSVersion) -> SupportedPlatform

Configures the minimum deployment target version for the tvOS platform.

static let tvOS: Platform

The tvOS platform.

struct TVOSVersion

The supported tvOS version.

