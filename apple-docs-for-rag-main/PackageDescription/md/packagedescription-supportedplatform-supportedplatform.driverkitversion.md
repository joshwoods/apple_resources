

- PackageDescription
- SupportedPlatform
-  SupportedPlatform.DriverKitVersion 

Structure

# SupportedPlatform.DriverKitVersion

The supported DriverKit version.

``` source
struct DriverKitVersion
```

## Topics

### Type Properties

static let v19: SupportedPlatform.DriverKitVersion

The value that represents DriverKit 19.0.

static let v20: SupportedPlatform.DriverKitVersion

The value that represents DriverKit 20.0.

static let v21: SupportedPlatform.DriverKitVersion

The value that represents DriverKit 21.0.

static let v22: SupportedPlatform.DriverKitVersion

The value that represents DriverKit 22.0.

static let v23: SupportedPlatform.DriverKitVersion

The value that represents DriverKit 23.0.

static let v24: SupportedPlatform.DriverKitVersion

The value that represents DriverKit 24.0.

## Relationships

### Conforms To

- Sendable

## See Also

### Supporting DriverKit

static func driverKit(SupportedPlatform.DriverKitVersion) -> SupportedPlatform

Configures the minimum deployment target version for the DriverKit platform.

static func driverKit(String) -> SupportedPlatform

Configures the minimum deployment target version for the DriverKit platform using a custom version string.

static let driverKit: Platform

The DriverKit platform

