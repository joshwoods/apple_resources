

- PackageDescription
-  SupportedPlatform 

Structure

# SupportedPlatform

A platform that the Swift package supports.

``` source
struct SupportedPlatform
```

## Overview

By default, Swift Package Manager assigns a predefined minimum deployment version for each supported platforms unless you configure supported platforms using the `platforms` API. This predefined deployment version is the oldest deployment target version that the installed SDK supports for a given platform. One exception to this rule is macOS, for which the minimum deployment target version starts from 10.10. Packages can choose to configure the minimum deployment target version for a platform by using the APIs defined in this struct. Swift Package Manager emits appropriate errors when an invalid value is provided for supported platforms, such as an empty array, multiple declarations for the same platform, or an invalid version specification.

Swift Package Manager emits an error if a dependency isn’t compatible with the top-level package’s deployment version. The deployment target of a package’s dependencies must be lower than or equal to the top-level package’s deployment target version for a particular platform.

## Topics

### Supporting iOS

static func iOS(SupportedPlatform.IOSVersion) -> SupportedPlatform

Configures the minimum deployment target version for the iOS platform.

static func iOS(String) -> SupportedPlatform

Configures the minimum deployment target version for the iOS platform using a custom version string.

static let iOS: Platform

The iOS platform.

struct IOSVersion

The supported iOS version.

### Supporting macOS

static func macOS(SupportedPlatform.MacOSVersion) -> SupportedPlatform

Configures the minimum deployment target version for the macOS platform.

static func macOS(String) -> SupportedPlatform

Configures the minimum deployment target version for the macOS platform using a version string.

static let macOS: Platform

The macOS platform.

struct MacOSVersion

The supported macOS version.

### Supporting watchOS

static func watchOS(SupportedPlatform.WatchOSVersion) -> SupportedPlatform

Configure the minimum deployment target version for the watchOS platform.

static func watchOS(String) -> SupportedPlatform

Configure the minimum deployment target version for the watchOS platform using a custom version string.

static let watchOS: Platform

The watchOS platform.

struct WatchOSVersion

The supported watchOS version.

### Supporting visionOS

static func visionOS(SupportedPlatform.VisionOSVersion) -> SupportedPlatform

Configure the minimum deployment target version for the visionOS platform.

static func visionOS(String) -> SupportedPlatform

Configure the minimum deployment target version for the visionOS platform using a custom version string.

static let visionOS: Platform

The visionOS platform.

struct VisionOSVersion

The supported visionOS version.

### Supporting tvOS

static func tvOS(SupportedPlatform.TVOSVersion) -> SupportedPlatform

Configures the minimum deployment target version for the tvOS platform.

static func tvOS(String) -> SupportedPlatform

Configures the minimum deployment target version for the tvOS platform using a custom version string.

static let tvOS: Platform

The tvOS platform.

struct TVOSVersion

The supported tvOS version.

### Supporting MacCatalyst

static func macCatalyst(SupportedPlatform.MacCatalystVersion) -> SupportedPlatform

Configures the minimum deployment target version for the Mac Catalyst platform.

static func macCatalyst(String) -> SupportedPlatform

Configures the minimum deployment target version for the Mac Catalyst platform using a version string.

static let macCatalyst: Platform

The Mac Catalyst platform.

struct MacCatalystVersion

The supported Mac Catalyst version.

### Supporting DriverKit

static func driverKit(SupportedPlatform.DriverKitVersion) -> SupportedPlatform

Configures the minimum deployment target version for the DriverKit platform.

static func driverKit(String) -> SupportedPlatform

Configures the minimum deployment target version for the DriverKit platform using a custom version string.

static let driverKit: Platform

The DriverKit platform

struct DriverKitVersion

The supported DriverKit version.

### Supporting Linux

static let linux: Platform

The Linux platform.

### Type methods

static func custom(String, versionString: String) -> SupportedPlatform

Configures the minimum deployment target version for custom platforms.

### Operator Functions

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (SupportedPlatform, SupportedPlatform) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Structures

struct CustomPlatformVersion

A supported custom platform version.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Declaring Supported Platforms

var platforms: [SupportedPlatform]?

The list of minimum versions for platforms supported by the package.

struct Platform

A platform supported by Swift Package Manager.

