

- PackageDescription
- SupportedPlatform
-  watchOS(\_:) 

Type Method

# watchOS(\_:)

Configure the minimum deployment target version for the watchOS platform.

``` source
static func watchOS(_ version: SupportedPlatform.WatchOSVersion) -> SupportedPlatform
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

### Supporting watchOS

static func watchOS(String) -> SupportedPlatform

Configure the minimum deployment target version for the watchOS platform using a custom version string.

static let watchOS: Platform

The watchOS platform.

struct WatchOSVersion

The supported watchOS version.

