

- HomeKit
-  HMCharacteristicTypeActiveIdentifier 

Global Variable

# HMCharacteristicTypeActiveIdentifier

An index that maps to the current active Input Source service.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
let HMCharacteristicTypeActiveIdentifier: String
```

## Discussion

This characteristic describes the current input source of a television by referencing the HMServiceTypeInputSource. The Active Identifier characteristic’s value should be a valid value within the identifiers of the Input Source service instances linked to the television service. The value of the characteristic is a `UInt32` integer.

## See Also

### Accessory identification

let HMCharacteristicTypeName: String

The name of the accessory.

let HMCharacteristicTypeIdentify: String

A control you can use to ask the accessory to identify itself.

let HMCharacteristicTypeVersion: String

The version of the accessory.

let HMCharacteristicTypeLogs: String

Log data for the accessory.

let HMCharacteristicTypeAdminOnlyAccess: String

An indicator of whether the accessory accepts only administrator access.

let HMCharacteristicTypeHardwareVersion: String

The hardware version of the accessory.

let HMCharacteristicTypeSoftwareVersion: String

The software version of the accessory.

let HMCharacteristicTypeLabelIndex: String

The index of the label for the service on an accessory with multiple instances of the same service.

let HMCharacteristicTypeLabelNamespace: String

The naming schema used to label the services on an accessory with multiple services of the same type.

let HMCharacteristicTypeIdentifier: String

The identifier for an accessory.

let HMCharacteristicTypeInputDeviceType: String

The accessory input device type.

let HMCharacteristicTypeInputSourceType: String

The accessory input source type.

let HMCharacteristicTypeConfiguredName: String

A `UTF‑8` encoded user visible name on an accessory.

