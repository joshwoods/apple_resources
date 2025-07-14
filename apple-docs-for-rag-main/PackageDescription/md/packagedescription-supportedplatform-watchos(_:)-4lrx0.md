

- PackageDescription
- SupportedPlatform
-  watchOS(\_:) 

Type Method

# watchOS(\_:)

Configure the minimum deployment target version for the watchOS platform using a custom version string.

``` source
static func watchOS(_ versionString: String) -> SupportedPlatform
```

## Parameters 

`versionString`  

The minimum deployment target as a string representation of two or three dot-separated integers, such as `2.0.1`.

## Return Value

A `SupportedPlatform` instance.

## Discussion

The version string must be a series of two or three dot-separated integers, such as `2.0` or `2.0.1`.

Since

First available in PackageDescription 5.0

## See Also

### Supporting watchOS

static func watchOS(SupportedPlatform.WatchOSVersion) -> SupportedPlatform

Configure the minimum deployment target version for the watchOS platform.

static let watchOS: Platform

The watchOS platform.

struct WatchOSVersion

The supported watchOS version.

