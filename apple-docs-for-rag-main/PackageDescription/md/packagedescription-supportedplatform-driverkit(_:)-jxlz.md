

- PackageDescription
- SupportedPlatform
-  driverKit(\_:) 

Type Method

# driverKit(\_:)

Configures the minimum deployment target version for the DriverKit platform.

SwiftPM 5.5+

``` source
static func driverKit(_ version: SupportedPlatform.DriverKitVersion) -> SupportedPlatform
```

## Parameters 

`version`  

The minimum deployment target that the package supports.

## See Also

### Supporting DriverKit

static func driverKit(String) -> SupportedPlatform

Configures the minimum deployment target version for the DriverKit platform using a custom version string.

static let driverKit: Platform

The DriverKit platform

struct DriverKitVersion

The supported DriverKit version.

