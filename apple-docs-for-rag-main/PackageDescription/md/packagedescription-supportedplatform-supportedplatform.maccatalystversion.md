

- PackageDescription
- SupportedPlatform
-  SupportedPlatform.MacCatalystVersion 

Structure

# SupportedPlatform.MacCatalystVersion

The supported Mac Catalyst version.

``` source
struct MacCatalystVersion
```

## Topics

### Type Properties

static let v13: SupportedPlatform.MacCatalystVersion

The value that represents Mac Catalyst 13.0.

static let v14: SupportedPlatform.MacCatalystVersion

The value that represents Mac Catalyst 14.0.

static let v15: SupportedPlatform.MacCatalystVersion

The value that represents Mac Catalyst 15.0.

static let v16: SupportedPlatform.MacCatalystVersion

The value that represents Mac Catalyst 16.0.

static let v17: SupportedPlatform.MacCatalystVersion

The value that represents Mac Catalyst 17.0.

static let v18: SupportedPlatform.MacCatalystVersion

The value that represents Mac Catalyst 18.0.

## Relationships

### Conforms To

- Sendable

## See Also

### Supporting MacCatalyst

static func macCatalyst(SupportedPlatform.MacCatalystVersion) -> SupportedPlatform

Configures the minimum deployment target version for the Mac Catalyst platform.

static func macCatalyst(String) -> SupportedPlatform

Configures the minimum deployment target version for the Mac Catalyst platform using a version string.

static let macCatalyst: Platform

The Mac Catalyst platform.

