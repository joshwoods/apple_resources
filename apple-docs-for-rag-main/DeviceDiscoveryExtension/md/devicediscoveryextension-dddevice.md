

- DeviceDiscoveryExtension
-  DDDevice 

Class

# DDDevice

An object that describes a discovered device of interest.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
class DDDevice
```

## Overview

The extension creates an instance of this class for a discovered device of interest and passes it to the system for display in the device picker UI (AVRoutePickerView).

The extension discovers devices through either Core Bluetooth or the local network (that is, using Bonjour).

For device discovery extensions of third-party media receivers, an instance of this class corresponds to the media receiver of interest.

The extension reports the status of discovered devices to the system using the report(_:) function, and it receives status updates about the device from the system by implementing didReceiveEvent(_:).

## Topics

### Initializing a device

init(displayName: String, category: DDDevice.Category, protocolType: UTType, identifier: String)

Creates an object that describes a discovered device.

### Identifying the device

var displayName: String

A name for the device to display to the user.

var identifier: String

A unique identifier for the device.

var category: DDDevice.Category

An option that determies the icon that the picker UI displays for the device.

enum Category

An option that determines the icon for the device in the picker UI.

### Indicating the protocol

var `protocol`: DDDevice.Protocol

The manner in which the system applies your app’s device discovery extension.

enum Protocol

An identifier for the manner in which an app interacts with a device.

var protocolType: UTType

A custom universal type that describes the device’s manner of communication with the extension.

var bluetoothIdentifier: UUID?

An identifier to communicate with the device through Bluetooth wireless technology.

var networkEndpoint: NWEndpoint?

An object that describes a local-network device.

### Setting the device state

var state: DDDeviceState

A state that represents the level of user interaction with the device.

var txtRecord: NWTXTRecord?

A dictionary of metadata for the device that the extension communicates with over the local network.

var url: URL

A resource locator for the simple service discovery protocol.

var supportsGrouping: Bool

A Boolean value that indicates whether to group the device with others in the AirPlay UI.

### Communicating device content and playback status

var mediaContentTitle: String?

A title for the current media that the device plays.

var mediaContentSubtitle: String?

A subtitle for the current media that the device plays.

var mediaPlaybackState: DDDevice.MediaPlaybackState

A playback status for the device’s current media.

enum MediaPlaybackState

States that indicate the status of a device’s media playback.

### Instance Properties

var deviceSupports: DDDeviceSupports

var displayImageName: String?

var ssid: String?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Device information

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

struct DDDeviceProtocolString

String values for the manner in which an app interacts with a device.

func DDDeviceMediaPlaybackStateToString(DDDevice.MediaPlaybackState) -> String

Returns human-readable text for the specified media playback state.

