

- DeviceDiscoveryExtension
-  DDDeviceProtocolString 

Structure

# DDDeviceProtocolString

String values for the manner in which an app interacts with a device.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
struct DDDeviceProtocolString
```

## Discussion

When an app creates a device discovery extension to stream content to a third-party media receiver, the protocol is Discovery and Launch (DIAL), as designated by the DDDevice.Protocol.dial option.

## Topics

### Creating a device protocol string

init(rawValue: String)

Creates a string for the manner in which an app interacts with a device.

### Specifying a device protocol string

static let dial: DDDeviceProtocolString

A human-readable string for the Discovery and Launch protocol.

static let invalid: DDDeviceProtocolString

A human-readable string for the default device protocol.

## Relationships

### Conforms To

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

enum DDDeviceState

A state that represents the level of user interaction with the device.

func DDDeviceCategoryToString(DDDevice.Category) -> String

Returns human-readable text for the specified identifier that describes a device’s category.

func DDDeviceStateToString(DDDeviceState) -> String

Returns human-readable text for the specified identifier that describes a device’s status.

enum Protocol

An identifier for the manner in which an app interacts with a device.

func DDDeviceProtocolToString(DDDevice.Protocol) -> String

Returns human-readable text for the specified protocol identifier.

func DDDeviceMediaPlaybackStateToString(DDDevice.MediaPlaybackState) -> String

Returns human-readable text for the specified media playback state.

