

- HealthKit
-  HKMetadataKeyDeviceSerialNumber 

Global Variable

# HKMetadataKeyDeviceSerialNumber

The key for the serial number of the device that generated the data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
let HKMetadataKeyDeviceSerialNumber: String
```

## Discussion

This key takes a string value.

## See Also

### Device Information Keys

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

enum HKDevicePlacementSide

Values that indicate the placement of the device that measured a sample.

let HKMetadataKeyAppleDeviceCalibrated: String

The key for metadata indicating whether the system had data from a sufficient amount of calibrated sensors when recording the sample.

