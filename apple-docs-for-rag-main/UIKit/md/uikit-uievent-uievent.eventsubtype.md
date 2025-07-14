

- UIKit
- UIEvent
-  UIEvent.EventSubtype 

Enumeration

# UIEvent.EventSubtype

Constants that specify the subtype of the event in relation to its general type.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum EventSubtype
```

## Overview

You can obtain the subtype of an event from the subtype property.

## Topics

### Constants

case none

The event has no subtype.

case motionShake

The event is related to a person shaking the device.

case remoteControlPlay

A remote-control event for playing audio or video.

case remoteControlPause

A remote-control event for pausing audio or video.

case remoteControlStop

A remote-control event for stopping audio or video from playing.

case remoteControlTogglePlayPause

A remote-control event for toggling audio or video between play and pause.

case remoteControlNextTrack

A remote-control event for skipping to the next audio or video track.

case remoteControlPreviousTrack

A remote-control event for skipping to the previous audio or video track.

case remoteControlBeginSeekingBackward

A remote-control event to start seeking backward through the audio or video medium.

case remoteControlEndSeekingBackward

A remote-control event to end seeking backward through the audio or video medium.

case remoteControlBeginSeekingForward

A remote-control event to start seeking forward through the audio or video medium.

case remoteControlEndSeekingForward

A remote-control event to end seeking forward through the audio or video medium.

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

### Getting the event type

var type: UIEvent.EventType

Returns the type of the event.

enum EventType

Constants that specify the general type of an event.

var subtype: UIEvent.EventSubtype

Returns the subtype of the event.

