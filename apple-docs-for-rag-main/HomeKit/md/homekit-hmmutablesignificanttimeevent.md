

- HomeKit
-  HMMutableSignificantTimeEvent 

Class

# HMMutableSignificantTimeEvent

A mutable event that fires at the specified temporal offset to a significant event.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class HMMutableSignificantTimeEvent
```

## Topics

### Configuring a significant time event

var significantEvent: HMSignificantEvent

The significant time-based event that is used to calculate when the event fires.

var offset: DateComponents

The offset from the significant event that this event fires at.

## Relationships

### Inherits From

- HMSignificantTimeEvent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- Sendable

## See Also

### Significant events

struct HMSignificantEvent

An event that represents significant time-based events, including sunrise and sunset.

class HMSignificantTimeEvent

An event that fires at a time offset from a significant time-based event.

