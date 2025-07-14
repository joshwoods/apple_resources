

- HealthKit
-  HKDevicePlacementSide 

Enumeration

# HKDevicePlacementSide

Values that indicate the placement of the device that measured a sample.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
enum HKDevicePlacementSide
```

## Topics

### Placements

case central

A device predominately located near the center of the body.

case left

A device predominately located on the left side.

case right

A device predominately located on the right side.

case unknown

The system couldn’t determine the device’s placement.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Device Information Keys

let HKMetadataKeyDeviceSerialNumber: String

The key for the serial number of the device that generated the data.

let HKMetadataKeyUDIDeviceIdentifier: String

The device identifier portion of a device’s UDI (unique device identifier).

let HKMetadataKeyUDIProductionIdentifier: String

The production identifier portion of a device’s UDI (unique device identifier).

let HKMetadataKeyDigitalSignature: String

A digital signature that can be used to validate the origin of the HealthKit object.

let HKMetadataKeyDeviceName: String

The name of the device that took this reading.

let HKMetadataKeyDeviceManufacturerName: String

The name of the manufacturer of the device that took this reading.

let HKMetadataKeyDevicePlacementSide: String

The key for metadata indicating the placement of the device that measured a sample.

let HKMetadataKeyAppleDeviceCalibrated: String

The key for metadata indicating whether the system had data from a sufficient amount of calibrated sensors when recording the sample.

