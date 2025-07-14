

- PackageDescription
- SupportedPlatform
-  macCatalyst(\_:) 

Type Method

# macCatalyst(\_:)

Configures the minimum deployment target version for the Mac Catalyst platform using a version string.

SwiftPM 5.5+

``` source
static func macCatalyst(_ versionString: String) -> SupportedPlatform
```

## Parameters 

`versionString`  

The minimum deployment target as a string representation of two or three dot-separated integers, such as `13.0.1`.

## Return Value

A `SupportedPlatform` instance.

## Discussion

The version string must be a series of two or three dot-separated integers, such as `13.0` or `13.0.1`.

Since

First available in PackageDescription 5.5

## See Also

### Supporting MacCatalyst

static func macCatalyst(SupportedPlatform.MacCatalystVersion) -> SupportedPlatform

Configures the minimum deployment target version for the Mac Catalyst platform.

static let macCatalyst: Platform

The Mac Catalyst platform.

struct MacCatalystVersion

The supported Mac Catalyst version.

