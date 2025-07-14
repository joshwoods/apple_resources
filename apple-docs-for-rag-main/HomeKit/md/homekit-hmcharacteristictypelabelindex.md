

- HomeKit
-  HMCharacteristicTypeLabelIndex 

Global Variable

# HMCharacteristicTypeLabelIndex

The index of the label for the service on an accessory with multiple instances of the same service.

iOS 10.3+iPadOS 10.3+Mac Catalyst 10.3+tvOS 10.2+visionOS 1.0+watchOS 3.2+

``` source
let HMCharacteristicTypeLabelIndex: String
```

## Discussion

The corresponding value is an integer that’s greater than or equal to `1`. When the value for the label namespace characteristic is HMCharacteristicValueLabelNamespace.dot, the label index indicates the number of dots, like `.`, `..`, `...`, and so on. When the value for the label namespace characteristic is HMCharacteristicValueLabelNamespace.numeral, the label index indicates the arabic numeral, like `1`, `2`, `3`, and so on.

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

let HMCharacteristicTypeLabelNamespace: String

The naming schema used to label the services on an accessory with multiple services of the same type.

let HMCharacteristicTypeActiveIdentifier: String

An index that maps to the current active Input Source service.

let HMCharacteristicTypeIdentifier: String

The identifier for an accessory.

let HMCharacteristicTypeInputDeviceType: String

The accessory input device type.

let HMCharacteristicTypeInputSourceType: String

The accessory input source type.

let HMCharacteristicTypeConfiguredName: String

A `UTF‑8` encoded user visible name on an accessory.

