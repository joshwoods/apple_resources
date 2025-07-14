

- EventKit
-  EKSpan 

Enumeration

# EKSpan

An object that indicates whether modifications should apply to a single event or all future events of a recurring event.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
enum EKSpan
```

## Topics

### Constants

case thisEvent

Modifications to this event instance should affect only this instance.

case futureEvents

Modifications to this event instance should also affect future instances of this event.

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

### Creating a Basic Recurrence Rule

init(recurrenceWith: EKRecurrenceFrequency, interval: Int, end: EKRecurrenceEnd?)

Initializes and returns a simple recurrence rule with a given frequency, interval, and end.

