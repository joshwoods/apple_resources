

- PackageDescription
-  Platform 

Structure

# Platform

A platform supported by Swift Package Manager.

``` source
struct Platform
```

## Topics

### Platforms

static let iOS: Platform

The iOS platform.

static let macOS: Platform

The macOS platform.

static let tvOS: Platform

The tvOS platform.

static let watchOS: Platform

The watchOS platform.

static let macCatalyst: Platform

The Mac Catalyst platform.

static let driverKit: Platform

The DriverKit platform

static let android: Platform

The Android platform.

static let linux: Platform

The Linux platform.

static let openbsd: Platform

The OpenBSD platform.

static let wasi: Platform

The WebAssembly System Interface platform.

static let windows: Platform

The Windows platform.

### Type methods

static func custom(String) -> Platform

Creates a custom platform.

### Operator Functions

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Operators

static func == (Platform, Platform) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Type Properties

static let visionOS: Platform

The visionOS platform.

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

struct SupportedPlatform

A platform that the Swift package supports.

