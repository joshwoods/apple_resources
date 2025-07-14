

- HomeKit
-  HMCharacteristicTypeConfiguredName 

Global Variable

# HMCharacteristicTypeConfiguredName

A `UTF‑8` encoded user visible name on an accessory.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
let HMCharacteristicTypeConfiguredName: String
```

## Overview

The `HMCharacteristicTypeConfiguredName` must not be defined as an empty string unless you define a nonempty `HMCharacteristicTypeName`. The initial value will be the current or default name that is set on the television. `HMCharacteristicTypeConfiguredName` is an editable text from either the accessory or the controller. When it’s an empty string, use HMCharacteristicTypeName as the name for this input source.

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

let HMCharacteristicTypeActiveIdentifier: String

An index that maps to the current active Input Source service.

let HMCharacteristicTypeIdentifier: String

The identifier for an accessory.

let HMCharacteristicTypeInputDeviceType: String

The accessory input device type.

let HMCharacteristicTypeInputSourceType: String

The accessory input source type.

