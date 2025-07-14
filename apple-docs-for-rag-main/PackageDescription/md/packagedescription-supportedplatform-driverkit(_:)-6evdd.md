

- PackageDescription
- SupportedPlatform
-  driverKit(\_:) 

Type Method

# driverKit(\_:)

Configures the minimum deployment target version for the DriverKit platform using a custom version string.

SwiftPM 5.5+

``` source
static func driverKit(_ versionString: String) -> SupportedPlatform
```

## Parameters 

`versionString`  

The minimum deployment target as a string representation of two or three dot-separated integers, such as `19.0.1`.

## Return Value

A `SupportedPlatform` instance.

## See Also

### Supporting DriverKit

static func driverKit(SupportedPlatform.DriverKitVersion) -> SupportedPlatform

Configures the minimum deployment target version for the DriverKit platform.

static let driverKit: Platform

The DriverKit platform

struct DriverKitVersion

The supported DriverKit version.

