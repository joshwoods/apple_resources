

- UIKit
- UIEvent
-  UIEvent.EventType 

Enumeration

# UIEvent.EventType

Constants that specify the general type of an event.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum EventType
```

## Overview

You can obtain the type of an event from the type property. To further identify the event, you might also need to determine its subtype, which you obtain from the subtype property.

## Topics

### Constants

case touches

The event relates to touches on the screen.

case motion

The event relates to motion of the device, such as when a person shakes it.

case remoteControl

The event is a remote-control event.

case presses

The event relates to the press of a physical button.

case scroll

The event relates to scrolling from an indirect input device.

case hover

The event relates to a pointer from an indirect input device moving over a user interface element.

case transform

The event relates to a pointer from an indirect input device performing a transformation on a user interface element, such as scaling, rotation, or translation.

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

var subtype: UIEvent.EventSubtype

Returns the subtype of the event.

enum EventSubtype

Constants that specify the subtype of the event in relation to its general type.

