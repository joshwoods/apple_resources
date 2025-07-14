

- HealthKit
-  HKMetadataKeyDigitalSignature 

Global Variable

# HKMetadataKeyDigitalSignature

A digital signature that can be used to validate the origin of the HealthKit object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
let HKMetadataKeyDigitalSignature: String
```

## Mentioned in 

Adding Digital Signatures

## Discussion

The digital signature is intended to provide data integrity for sample data produced by trusted (tamper resistant) measuring devices. Use the Cryptographic Message Syntax (CMS) to sign data returned by your device (such as timestamps, values, and so forth) using ASN.1 encoding with Distinguished Encoding Rules (DER). The entire signature should be further encoded using base64. Recommended digest is SHA256, and recommended cipher is FIPS PUB 186-4 Digital Signature Standard Elliptic Curve P-256. CMS is specified in IETF RFC 5652. For more information, see Adding Digital Signatures in `HealthKit`.

## See Also

### Device Information Keys

let HKMetadataKeyDeviceSerialNumber: String

The key for the serial number of the device that generated the data.

let HKMetadataKeyUDIDeviceIdentifier: String

The device identifier portion of a device’s UDI (unique device identifier).

let HKMetadataKeyUDIProductionIdentifier: String

The production identifier portion of a device’s UDI (unique device identifier).

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

