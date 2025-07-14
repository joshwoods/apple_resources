

- PackageDescription
- SupportedPlatform
-  SupportedPlatform.IOSVersion 

Structure

# SupportedPlatform.IOSVersion

The supported iOS version.

``` source
struct IOSVersion
```

## Topics

### Type Properties

static let v10: SupportedPlatform.IOSVersion

The value that represents iOS 10.0.

Deprecated

static let v11: SupportedPlatform.IOSVersion

The value that represents iOS 11.0.

Deprecated

static let v12: SupportedPlatform.IOSVersion

The value that represents iOS 12.0.

static let v13: SupportedPlatform.IOSVersion

The value that represents iOS 13.0.

static let v14: SupportedPlatform.IOSVersion

The value that represents iOS 14.0.

static let v15: SupportedPlatform.IOSVersion

The value that represents iOS 15.0.

static let v16: SupportedPlatform.IOSVersion

The value that represents iOS 16.0.

static let v17: SupportedPlatform.IOSVersion

The value that represents iOS 17.0.

static let v18: SupportedPlatform.IOSVersion

The value that represents iOS 18.0.

static let v8: SupportedPlatform.IOSVersion

The value that represents iOS 8.0.

Deprecated

static let v9: SupportedPlatform.IOSVersion

The value that represents iOS 9.0.

Deprecated

## Relationships

### Conforms To

- Sendable

## See Also

### Supporting iOS

static func iOS(SupportedPlatform.IOSVersion) -> SupportedPlatform

Configures the minimum deployment target version for the iOS platform.

static func iOS(String) -> SupportedPlatform

Configures the minimum deployment target version for the iOS platform using a custom version string.

static let iOS: Platform

The iOS platform.

