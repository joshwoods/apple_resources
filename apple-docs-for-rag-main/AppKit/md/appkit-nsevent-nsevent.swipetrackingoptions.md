

- AppKit
- NSEvent
-  NSEvent.SwipeTrackingOptions 

Structure

# NSEvent.SwipeTrackingOptions

Constants that specify swipe-tracking options.

macOS 10.7+

``` source
struct SwipeTrackingOptions
```

## Topics

### Constants

static var lockDirection: NSEvent.SwipeTrackingOptions

Clamp gestureAmount to 0 if the user starts to swipe in the opposite direction than they started.

static var clampGestureAmount: NSEvent.SwipeTrackingOptions

Don’t allow gestureAmount to go beyond +/-1.0

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

struct ButtonMask

Constants you use to identify the activated tablet buttons in an event.

struct ModifierFlags

Flags that represent key states in an event object.

struct Phase

Constants that represent the possible phases during an event phase.

init(type: NSEvent.EventType)

Returns the event mask for the specified type.

