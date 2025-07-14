

- Core Bluetooth
- CBCentralManager
-  CBCentralManager.Feature 

Structure

# CBCentralManager.Feature

An option set of device-specific features.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
struct Feature
```

## Topics

### Creating a Central Manager Feature Instance

init(rawValue: UInt)

Creates a central manager feature instance.

### Extended Scan Features

static var extendedScanAndConnect: CBCentralManager.Feature

The hardware supports extended scans and enhanced connection creation.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Inspecting Feature Support

class func supports(CBCentralManager.Feature) -> Bool

Returns a Boolean that indicates whether the device supports a specific set of features.

