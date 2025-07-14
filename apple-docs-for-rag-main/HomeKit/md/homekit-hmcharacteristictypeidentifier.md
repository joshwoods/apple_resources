

- HomeKit
-  HMCharacteristicTypeIdentifier 

Global Variable

# HMCharacteristicTypeIdentifier

The identifier for an accessory.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
let HMCharacteristicTypeIdentifier: String
```

## Overview

In the Input Source Ordering Profile, `HMCharacteristicTypeIdentifier` identifies an instance of the Input Source service. The value for each instance of this service must be unique within the list of input source services linked to a television service. A value of `0` isn’t valid for the instance of this characteristic included in the Input Source service.

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

let HMCharacteristicTypeInputDeviceType: String

The accessory input device type.

let HMCharacteristicTypeInputSourceType: String

The accessory input source type.

let HMCharacteristicTypeConfiguredName: String

A `UTF‑8` encoded user visible name on an accessory.

