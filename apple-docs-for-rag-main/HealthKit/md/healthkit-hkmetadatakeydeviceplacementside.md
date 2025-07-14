

- HealthKit
-  HKMetadataKeyDevicePlacementSide 

Global Variable

# HKMetadataKeyDevicePlacementSide

The key for metadata indicating the placement of the device that measured a sample.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
let HKMetadataKeyDevicePlacementSide: String
```

## Discussion

This key takes an NSNumber that contains a value from HKDevicePlacementSide.

For mobility samples, like walkingSpeed or walkingDoubleSupportPercentage, this metadata key records the placement of the device as determined by the system.

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

enum HKDevicePlacementSide

Values that indicate the placement of the device that measured a sample.

let HKMetadataKeyAppleDeviceCalibrated: String

The key for metadata indicating whether the system had data from a sufficient amount of calibrated sensors when recording the sample.

