

- PackageDescription
- SupportedPlatform
-  SupportedPlatform.TVOSVersion 

Structure

# SupportedPlatform.TVOSVersion

The supported tvOS version.

``` source
struct TVOSVersion
```

## Topics

### Type Properties

static let v10: SupportedPlatform.TVOSVersion

The value that represents tvOS 10.0.

Deprecated

static let v11: SupportedPlatform.TVOSVersion

The value that represents tvOS 11.0.

Deprecated

static let v12: SupportedPlatform.TVOSVersion

The value that represents tvOS 12.0.

static let v13: SupportedPlatform.TVOSVersion

The value that represents tvOS 13.0.

static let v14: SupportedPlatform.TVOSVersion

The value that represents tvOS 14.0.

static let v15: SupportedPlatform.TVOSVersion

The value that represents tvOS 15.0.

static let v16: SupportedPlatform.TVOSVersion

The value that represents tvOS 16.0.

static let v17: SupportedPlatform.TVOSVersion

The value that represents tvOS 17.0.

static let v18: SupportedPlatform.TVOSVersion

The value that represents tvOS 18.0.

static let v9: SupportedPlatform.TVOSVersion

The value that represents tvOS 9.0.

Deprecated

## Relationships

### Conforms To

- Sendable

## See Also

### Supporting tvOS

static func tvOS(SupportedPlatform.TVOSVersion) -> SupportedPlatform

Configures the minimum deployment target version for the tvOS platform.

static func tvOS(String) -> SupportedPlatform

Configures the minimum deployment target version for the tvOS platform using a custom version string.

static let tvOS: Platform

The tvOS platform.

