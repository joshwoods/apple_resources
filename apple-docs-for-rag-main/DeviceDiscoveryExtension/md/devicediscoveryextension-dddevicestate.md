

- DeviceDiscoveryExtension
-  DDDeviceState 

Enumeration

# DDDeviceState

A state that represents the level of user interaction with the device.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
enum DDDeviceState
```

## Overview

The device (DDDevice) state property is of this type.

## Topics

### Communicating a device’s status

case invalid

A state that indicates the device is invalid or that the user disapproves of the device.

case activating

A state that indicates when the user selects the device in the picker UI.

case activated

A state that indicates when the user authorizes the device and the app connects to the device.

case authorized

A state that indicates when the user authorizes the device.

case invalidating

A state that indicates that the device is soon to be invalid.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Device information

class DDDevice

An object that describes a discovered device of interest.

enum Category

An option that determines the icon for the device in the picker UI.

func DDDeviceCategoryToString(DDDevice.Category) -> String

Returns human-readable text for the specified identifier that describes a device’s category.

func DDDeviceStateToString(DDDeviceState) -> String

Returns human-readable text for the specified identifier that describes a device’s status.

enum Protocol

An identifier for the manner in which an app interacts with a device.

func DDDeviceProtocolToString(DDDevice.Protocol) -> String

Returns human-readable text for the specified protocol identifier.

struct DDDeviceProtocolString

String values for the manner in which an app interacts with a device.

func DDDeviceMediaPlaybackStateToString(DDDevice.MediaPlaybackState) -> String

Returns human-readable text for the specified media playback state.

