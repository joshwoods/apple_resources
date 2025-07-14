

- DeviceDiscoveryExtension
- DDDevice
-  DDDevice.Category 

Enumeration

# DDDevice.Category

An option that determines the icon for the device in the picker UI.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
enum Category
```

## Overview

The device (DDDevice) category property is of this type.

Each value in this enumeration determines a different icon that the picker UI (AVRoutePickerView) displays, which helps the user visually confirm that their selection corresponds to the device they intend to stream media to.

## Topics

### Choosing an icon for the device picker

case desktopComputer

An icon that depicts a desktop computer.

case hifiSpeaker

An icon that depicts a high-fidelity speaker.

case hifiSpeakerMultiple

An icon that depicts multiple high-fidelity speakers.

case laptopComputer

An icon that depicts a laptop computer.

case tv

An icon that depicts a television.

case tvWithMediaBox

An icon that depicts a TV with a set-top box.

### Enumeration Cases

case accessorySetup

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

