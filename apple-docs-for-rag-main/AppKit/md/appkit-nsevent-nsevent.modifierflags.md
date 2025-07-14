

- AppKit
- NSEvent
-  NSEvent.ModifierFlags 

Structure

# NSEvent.ModifierFlags

Flags that represent key states in an event object.

macOS

``` source
struct ModifierFlags
```

## Topics

### Event Modifier Flags

static var capsLock: NSEvent.ModifierFlags

The Caps Lock key has been pressed.

static var shift: NSEvent.ModifierFlags

The Shift key has been pressed.

static var control: NSEvent.ModifierFlags

The Control key has been pressed.

static var option: NSEvent.ModifierFlags

The Option or Alt key has been pressed.

static var command: NSEvent.ModifierFlags

The Command key has been pressed.

static var numericPad: NSEvent.ModifierFlags

A key in the numeric keypad or an arrow key has been pressed.

static var help: NSEvent.ModifierFlags

The Help key has been pressed.

static var function: NSEvent.ModifierFlags

A function key has been pressed.

static var deviceIndependentFlagsMask: NSEvent.ModifierFlags

Device-independent modifier flags are masked.

### Deprecated

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

struct ButtonMask

Constants you use to identify the activated tablet buttons in an event.

struct Phase

Constants that represent the possible phases during an event phase.

struct SwipeTrackingOptions

Constants that specify swipe-tracking options.

init(type: NSEvent.EventType)

Returns the event mask for the specified type.

