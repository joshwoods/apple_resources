

- HomeKit
-  HMCharacteristicTypeStatusFault 

Global Variable

# HMCharacteristicTypeStatusFault

An indicator of whether the accessory has experienced a fault.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
let HMCharacteristicTypeStatusFault: String
```

## Discussion

The corresponding value is one of the constants in the HMCharacteristicValueStatusFault enumeration. It indicates whether the accessory has experienced a fault that interferes with normal functioning, such as when a humidifier runs out of water.

## Topics

### Values

enum HMCharacteristicValueStatusFault

Possible values for the fault status of an accessory.

## See Also

### General state

let HMCharacteristicTypeActive: String

The current status of an accessory.

let HMCharacteristicTypeStatusTampered: String

An indicator of whether an accessory has been tampered with.

let HMCharacteristicTypeStatusActive: String

An indicator of whether the service is working.

let HMCharacteristicTypeInUse: String

The current usage state of an accessory.

let HMCharacteristicTypeIsConfigured: String

The configuration state of an accessory.

let HMCharacteristicTypeRemainingDuration: String

The number of seconds remaining for the activity being carried out by the accessory.

let HMCharacteristicTypeSetDuration: String

The duration of the activity being carried out by the accessory.

let HMCharacteristicTypeProgramMode: String

The current mode of the accessory’s scheduled programs.

let HMCharacteristicTypeWiFiSatelliteStatus: String

The network status of the WiFi satellite accessory.

let HMCharacteristicTypeWANStatusList: String

The WAN status list of an accessory.

let HMCharacteristicTypeTargetMediaState: String

The target media state.

let HMCharacteristicTypeRouterStatus: String

The current status of the router.

let HMCharacteristicTypeCurrentMediaState: String

The current state of the media.

let HMCharacteristicTypeCurrentVisibilityState: String

The current visibility state for a service.

let HMCharacteristicTypeTargetVisibilityState: String

The target visibility state for a service.

