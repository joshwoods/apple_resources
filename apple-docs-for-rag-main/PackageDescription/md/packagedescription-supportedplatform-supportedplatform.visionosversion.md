

- PackageDescription
- SupportedPlatform
-  SupportedPlatform.VisionOSVersion 

Structure

# SupportedPlatform.VisionOSVersion

The supported visionOS version.

``` source
struct VisionOSVersion
```

## Topics

### Type Properties

static let v1: SupportedPlatform.VisionOSVersion

The value that represents visionOS 1.0.

static let v2: SupportedPlatform.VisionOSVersion

The value that represents visionOS 2.0.

## Relationships

### Conforms To

- Sendable

## See Also

### Supporting visionOS

static func visionOS(SupportedPlatform.VisionOSVersion) -> SupportedPlatform

Configure the minimum deployment target version for the visionOS platform.

static func visionOS(String) -> SupportedPlatform

Configure the minimum deployment target version for the visionOS platform using a custom version string.

static let visionOS: Platform

The visionOS platform.

