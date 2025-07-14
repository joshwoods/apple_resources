

- AppKit
- NSEvent
-  NSEvent.ButtonMask 

Structure

# NSEvent.ButtonMask

Constants you use to identify the activated tablet buttons in an event.

macOS

``` source
struct ButtonMask
```

## Topics

### Getting the Tablet Button Masks

static var penTip: NSEvent.ButtonMask

A mask that matches the pen tip.

static var penLowerSide: NSEvent.ButtonMask

A mask that matches the button on the lower side of the device.

static var penUpperSide: NSEvent.ButtonMask

A mask that matches the button on the upper side of the device.

### Initializers

init(rawValue: UInt)

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

struct EventTypeMask

Constants that you use to filter out specific event types from the stream of incoming events.

struct ModifierFlags

Flags that represent key states in an event object.

struct Phase

Constants that represent the possible phases during an event phase.

struct SwipeTrackingOptions

Constants that specify swipe-tracking options.

init(type: NSEvent.EventType)

Returns the event mask for the specified type.

