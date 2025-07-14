

- HealthKit
-  HKMetadataKeyUDIDeviceIdentifier 

Global Variable

# HKMetadataKeyUDIDeviceIdentifier

The device identifier portion of a device’s UDI (unique device identifier).

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
let HKMetadataKeyUDIDeviceIdentifier: String
```

## Discussion

The device identifier can be used to reference the GUDID (Globally Unique Device Identification Database).

This key takes a string value.

Note

In iOS 9.0 and later, the use of this key is discouraged. Use the HKDevice class instead.

## See Also

### Device Information Keys

let HKMetadataKeyDeviceSerialNumber: String

The key for the serial number of the device that generated the data.

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

