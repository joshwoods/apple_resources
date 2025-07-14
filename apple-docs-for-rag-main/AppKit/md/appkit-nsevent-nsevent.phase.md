

- AppKit
- NSEvent
-  NSEvent.Phase 

Structure

# NSEvent.Phase

Constants that represent the possible phases during an event phase.

macOS 10.7+

``` source
struct Phase
```

## Topics

### Constants

static var began: NSEvent.Phase

An event phase has begun.

static var stationary: NSEvent.Phase

An event phase is in progress but hasn’t moved since the previous event.

static var changed: NSEvent.Phase

An event phase has changed.

static var ended: NSEvent.Phase

The event phase ended.

static var cancelled: NSEvent.Phase

The system canceled the event phase.

static var mayBegin: NSEvent.Phase

The system event phase may begin.

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

struct SwipeTrackingOptions

Constants that specify swipe-tracking options.

init(type: NSEvent.EventType)

Returns the event mask for the specified type.

