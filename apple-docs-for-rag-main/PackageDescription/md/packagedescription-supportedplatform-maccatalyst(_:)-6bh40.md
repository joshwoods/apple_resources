

- PackageDescription
- SupportedPlatform
-  macCatalyst(\_:) 

Type Method

# macCatalyst(\_:)

Configures the minimum deployment target version for the Mac Catalyst platform.

SwiftPM 5.5+

``` source
static func macCatalyst(_ version: SupportedPlatform.MacCatalystVersion) -> SupportedPlatform
```

## Parameters 

`version`  

The minimum deployment target that the package supports.

## Return Value

A `SupportedPlatform` instance.

## Discussion

Since

First available in PackageDescription 5.5

## See Also

### Supporting MacCatalyst

static func macCatalyst(String) -> SupportedPlatform

Configures the minimum deployment target version for the Mac Catalyst platform using a version string.

static let macCatalyst: Platform

The Mac Catalyst platform.

struct MacCatalystVersion

The supported Mac Catalyst version.

