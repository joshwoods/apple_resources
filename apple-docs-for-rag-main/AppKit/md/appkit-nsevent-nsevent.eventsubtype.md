

- AppKit
- NSEvent
-  NSEvent.EventSubtype 

Enumeration

# NSEvent.EventSubtype

Subtypes for various types of events.

macOS

``` source
enum EventSubtype
```

## Overview

The event subtype contains one of these constants only when the event’s type property contains NSAppKitDefined, NSSystemDefined, or NSApplicationDefined or a mouse-related event type.

## Topics

### Getting AppKit Event Subtypes

These subtypes apply when the event type is NSEvent.EventType.appKitDefined.

case applicationActivated

An app-activation event occurred.

case applicationDeactivated

An app-deactivation event occurred.

case screenChanged

An event that indicates a window changed screens.

case windowExposed

An event that indicates a window’s contents are visible again.

case windowMoved

An event that indicates a window moved.

### Getting System Event Subtypes

This subtype applies when the event type is NSEvent.EventType.systemDefined.

static var powerOff: NSEvent.EventSubtype

An event that indicates a system shutdown or restart operation is in progress.

static var powerOff: NSEvent.EventSubtype

An event that indicates a system shutdown or restart operation is in progress.

### Getting Other Subtypes

static var mouseEvent: NSEvent.EventSubtype

A mouse event occurred.

static var tabletPoint: NSEvent.EventSubtype

A tablet-pointer event occurred.

static var tabletProximity: NSEvent.EventSubtype

A tablet-proximity event occurred.

case touch

A touch event occurred.

### Initializers

init?(rawValue: Int16)

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

enum EventType

Constants for the types of events that responder objects can handle.

struct EventTypeMask

Constants that you use to filter out specific event types from the stream of incoming events.

var subtype: NSEvent.EventSubtype

The event’s subtype.

