

- DeviceDiscoveryExtension
- DDDevice
-  DDDevice.MediaPlaybackState 

Enumeration

# DDDevice.MediaPlaybackState

States that indicate the status of a device’s media playback.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
enum MediaPlaybackState
```

## Overview

The device (DDDevice) property mediaPlaybackState is of this type.

## Topics

### Distinguishing media playback states

case noContent

A state that indicates when the device plays no content.

case paused

A state that indicates when content playback for the device pauses.

case playing

A state that indicates when the device plays media.

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

### Communicating device content and playback status

var mediaContentTitle: String?

A title for the current media that the device plays.

var mediaContentSubtitle: String?

A subtitle for the current media that the device plays.

var mediaPlaybackState: DDDevice.MediaPlaybackState

A playback status for the device’s current media.

