

- PackageDescription
- SupportedPlatform
-  SupportedPlatform.MacOSVersion 

Structure

# SupportedPlatform.MacOSVersion

The supported macOS version.

``` source
struct MacOSVersion
```

## Topics

### Type Properties

static let v10_10: SupportedPlatform.MacOSVersion

The value that represents macOS 10.10.

Deprecated

static let v10_11: SupportedPlatform.MacOSVersion

The value that represents macOS 10.11.

Deprecated

static let v10_12: SupportedPlatform.MacOSVersion

The value that represents macOS 10.12.

Deprecated

static let v10_13: SupportedPlatform.MacOSVersion

The value that represents macOS 10.13.

static let v10_14: SupportedPlatform.MacOSVersion

The value that represents macOS 10.14.

static let v10_15: SupportedPlatform.MacOSVersion

The value that represents macOS 10.15.

static let v11: SupportedPlatform.MacOSVersion

The value that represents macOS 11.0.

static let v12: SupportedPlatform.MacOSVersion

The value that represents macOS 12.0.

static let v13: SupportedPlatform.MacOSVersion

The value that represents macOS 13.0.

static let v14: SupportedPlatform.MacOSVersion

The value that represents macOS 14.0.

static let v15: SupportedPlatform.MacOSVersion

The value that represents macOS 15.0.

## Relationships

### Conforms To

- Sendable

## See Also

### Supporting macOS

static func macOS(SupportedPlatform.MacOSVersion) -> SupportedPlatform

Configures the minimum deployment target version for the macOS platform.

static func macOS(String) -> SupportedPlatform

Configures the minimum deployment target version for the macOS platform using a version string.

static let macOS: Platform

The macOS platform.

