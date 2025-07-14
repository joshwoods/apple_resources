

- AppKit
- NSEvent
-  NSEvent.EventTypeMask 

Structure

# NSEvent.EventTypeMask

Constants that you use to filter out specific event types from the stream of incoming events.

macOS

``` source
struct EventTypeMask
```

## Overview

Pass these constants to the NSCell method sendAction(on:) to specify when an NSCell object should send its action message.

## Topics

### Getting Any Event

static var any: NSEvent.EventTypeMask

A mask that matches any type of event.

### Getting Mouse-Related Events

static var leftMouseDown: NSEvent.EventTypeMask

A mask for left mouse-down events.

static var leftMouseDragged: NSEvent.EventTypeMask

A mask for left mouse-dragged events.

static var leftMouseUp: NSEvent.EventTypeMask

A mask for left mouse-up events.

static var rightMouseDown: NSEvent.EventTypeMask

A mask for right mouse-down events.

static var rightMouseDragged: NSEvent.EventTypeMask

A mask for right mouse-dragged events.

static var rightMouseUp: NSEvent.EventTypeMask

A mask for right mouse-up events.

static var otherMouseDown: NSEvent.EventTypeMask

A mask for tertiary mouse-down events.

static var otherMouseDragged: NSEvent.EventTypeMask

A mask for tertiary mouse-dragged events.

static var otherMouseUp: NSEvent.EventTypeMask

A mask for tertiary mouse-up events.

static var mouseEntered: NSEvent.EventTypeMask

A mask for mouse-entered events.

static var mouseMoved: NSEvent.EventTypeMask

A mask for mouse-moved events.

static var mouseExited: NSEvent.EventTypeMask

A mask for mouse-exited events.

### Getting Keyboard Events

static var keyDown: NSEvent.EventTypeMask

A mask for key-down events.

static var keyUp: NSEvent.EventTypeMask

A mask for key-up events.

### Getting Touch Events

static var beginGesture: NSEvent.EventTypeMask

A mask for begin-gesture events.

static var endGesture: NSEvent.EventTypeMask

A mask for end-gesture events.

static var magnify: NSEvent.EventTypeMask

A mask for magnify-gesture events.

static var smartMagnify: NSEvent.EventTypeMask

A mask for smart-zoom gesture events.

static var swipe: NSEvent.EventTypeMask

A mask for swipe-gesture events.

static var rotate: NSEvent.EventTypeMask

A mask for rotate-gesture events.

static var gesture: NSEvent.EventTypeMask

A mask for generic gesture events.

static var directTouch: NSEvent.EventTypeMask

A mask for touch events.

static var tabletPoint: NSEvent.EventTypeMask

A mask for tablet-point events.

static var tabletProximity: NSEvent.EventTypeMask

A mask for tablet-proximity events.

static var pressure: NSEvent.EventTypeMask

A mask for pressure-change events.

### Getting Input Events

static var scrollWheel: NSEvent.EventTypeMask

A mask for scroll-wheel events.

static var changeMode: NSEvent.EventTypeMask

A mask for change-mode events.

### Getting System Events

static var appKitDefined: NSEvent.EventTypeMask

A mask for AppKit–defined events.

static var applicationDefined: NSEvent.EventTypeMask

A mask for app-defined events.

static var cursorUpdate: NSEvent.EventTypeMask

A mask for cursor-update events.

static var flagsChanged: NSEvent.EventTypeMask

A mask for flags-changed events.

static var periodic: NSEvent.EventTypeMask

A mask for periodic events.

static var systemDefined: NSEvent.EventTypeMask

A mask for system-defined events.

### Creating an Event Mask

init(rawValue: UInt64)

init(type: NSEvent.EventType)

Returns the event mask for the specified type.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Constants

struct ButtonMask

Constants you use to identify the activated tablet buttons in an event.

struct ModifierFlags

Flags that represent key states in an event object.

struct Phase

Constants that represent the possible phases during an event phase.

struct SwipeTrackingOptions

Constants that specify swipe-tracking options.

init(type: NSEvent.EventType)

Returns the event mask for the specified type.

