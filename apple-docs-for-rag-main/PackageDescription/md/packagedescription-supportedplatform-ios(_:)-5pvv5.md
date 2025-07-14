

- PackageDescription
- SupportedPlatform
-  iOS(\_:) 

Type Method

# iOS(\_:)

Configures the minimum deployment target version for the iOS platform.

``` source
static func iOS(_ version: SupportedPlatform.IOSVersion) -> SupportedPlatform
```

## Parameters 

`version`  

The minimum deployment target that the package supports.

## Return Value

A `SupportedPlatform` instance.

## Discussion

Since

First available in PackageDescription 5.0.

## See Also

### Supporting iOS

static func iOS(String) -> SupportedPlatform

Configures the minimum deployment target version for the iOS platform using a custom version string.

static let iOS: Platform

The iOS platform.

struct IOSVersion

The supported iOS version.

