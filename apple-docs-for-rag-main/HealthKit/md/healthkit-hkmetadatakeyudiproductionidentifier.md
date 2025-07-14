

- HealthKit
-  HKMetadataKeyUDIProductionIdentifier 

Global Variable

# HKMetadataKeyUDIProductionIdentifier

The production identifier portion of a device’s UDI (unique device identifier).

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
let HKMetadataKeyUDIProductionIdentifier: String
```

## Discussion

Although the production identifier is part of a device’s UDI, it is not saved in the FDA’s GUDID (Globally Unique Device Identifier Database), and its use in HealthKit is now discouraged to protect user privacy. Apps that need this information should store it outside the HealthKit store.

## See Also

### Device Information Keys

let HKMetadataKeyDeviceSerialNumber: String

The key for the serial number of the device that generated the data.

let HKMetadataKeyUDIDeviceIdentifier: String

The device identifier portion of a device’s UDI (unique device identifier).

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

