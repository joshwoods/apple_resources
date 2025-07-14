

- AppKit
- NSEvent
-  NSEvent.EventType 

Enumeration

# NSEvent.EventType

Constants for the types of events that responder objects can handle.

macOS

``` source
enum EventType
```

## Overview

These constants appear in the event’s type property. You also use them when you construct new events.

## Topics

### Getting Mouse-Related Event Types

case leftMouseDown

The user pressed the left mouse button.

case leftMouseDragged

The user moved the mouse while holding down the left mouse button.

case leftMouseUp

The user released the left mouse button.

case rightMouseDown

The user pressed the right mouse button.

case rightMouseUp

The user released the right mouse button.

case rightMouseDragged

The user moved the mouse while holding down the right mouse button.

case otherMouseDown

The user pressed a tertiary mouse button.

case otherMouseDragged

The user moved the mouse while holding down a tertiary mouse button.

case otherMouseUp

The user released a tertiary mouse button.

case mouseMoved

The user moved the mouse in a way that caused the cursor to move onscreen.

case mouseEntered

The cursor entered a well-defined area, such as a view.

case mouseExited

The cursor exited a well-defined area, such as a view.

### Getting Keyboard Event Types

case keyDown

The user pressed a key on the keyboard.

case keyUp

The user released a key on the keyboard.

### Getting Touch-Based Events

case beginGesture

An event marking the beginning of a gesture.

case endGesture

An event that marks the end of a gesture.

case magnify

The user performed a pinch-open or pinch-close gesture.

case smartMagnify

The user performed a smart-zoom gesture.

case swipe

The user performed a swipe gesture.

case rotate

The user performed a rotate gesture.

case gesture

The user performed a nonspecific type of gesture.

case directTouch

The user touched a portion of the touch bar.

case tabletPoint

The user touched a point on a tablet.

case tabletProximity

A pointing device is near, but not touching, the associated tablet.

case pressure

An event that reports a change in pressure on a pressure-sensitive device.

### Getting Other Input Types

case scrollWheel

The scroll wheel position changed.

case changeMode

The user changed the mode of a connected device.

### Getting System Event Types

case appKitDefined

An AppKit-related event occurred.

case applicationDefined

An app-defined event occurred.

case cursorUpdate

An event that updates the cursor.

case flagsChanged

The event flags changed.

case periodic

An event that provides execution time to periodic tasks.

case quickLook

An event that initiates a Quick Look request.

case systemDefined

A system-related event occurred.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the event type

var type: NSEvent.EventType

The event’s type.

struct EventTypeMask

Constants that you use to filter out specific event types from the stream of incoming events.

var subtype: NSEvent.EventSubtype

The event’s subtype.

enum EventSubtype

Subtypes for various types of events.

