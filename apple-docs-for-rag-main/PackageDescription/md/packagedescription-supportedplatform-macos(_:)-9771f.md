

- PackageDescription
- SupportedPlatform
-  macOS(\_:) 

Type Method

# macOS(\_:)

Configures the minimum deployment target version for the macOS platform using a version string.

``` source
static func macOS(_ versionString: String) -> SupportedPlatform
```

## Parameters 

`versionString`  

The minimum deployment target as a string representation of two or three dot-separated integers, such as `10.10.1`.

## Return Value

A `SupportedPlatform` instance.

## Discussion

The version string must be a series of two or three dot-separated integers, such as `10.10` or `10.10.1`.

Since

First available in PackageDescription 5.0.

## See Also

### Supporting macOS

static func macOS(SupportedPlatform.MacOSVersion) -> SupportedPlatform

Configures the minimum deployment target version for the macOS platform.

static let macOS: Platform

The macOS platform.

struct MacOSVersion

The supported macOS version.

