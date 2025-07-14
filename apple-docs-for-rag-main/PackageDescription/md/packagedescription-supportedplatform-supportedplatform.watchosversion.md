

- PackageDescription
- SupportedPlatform
-  SupportedPlatform.WatchOSVersion 

Structure

# SupportedPlatform.WatchOSVersion

The supported watchOS version.

``` source
struct WatchOSVersion
```

## Topics

### Type Properties

static let v10: SupportedPlatform.WatchOSVersion

The value that represents watchOS 10.0.

static let v11: SupportedPlatform.WatchOSVersion

The value that represents watchOS 11.0.

static let v2: SupportedPlatform.WatchOSVersion

The value that represents watchOS 2.0.

Deprecated

static let v3: SupportedPlatform.WatchOSVersion

The value that represents watchOS 3.0.

Deprecated

static let v4: SupportedPlatform.WatchOSVersion

The value that represents watchOS 4.0.

static let v5: SupportedPlatform.WatchOSVersion

The value that represents watchOS 5.0.

static let v6: SupportedPlatform.WatchOSVersion

The value that represents watchOS 6.0.

static let v7: SupportedPlatform.WatchOSVersion

The value that represents watchOS 7.0.

static let v8: SupportedPlatform.WatchOSVersion

The value that represents watchOS 8.0.

static let v9: SupportedPlatform.WatchOSVersion

The value that represents watchOS 9.0.

## Relationships

### Conforms To

- Sendable

## See Also

### Supporting watchOS

static func watchOS(SupportedPlatform.WatchOSVersion) -> SupportedPlatform

Configure the minimum deployment target version for the watchOS platform.

static func watchOS(String) -> SupportedPlatform

Configure the minimum deployment target version for the watchOS platform using a custom version string.

static let watchOS: Platform

The watchOS platform.

