

- HomeKit
-  HMCalendarEvent 

Class

# HMCalendarEvent

An event that fires at a specified time.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class HMCalendarEvent
```

## Topics

### Creating a calendar event

init(fire: DateComponents)

Creates a calendar event which fires based on the value of the supplied date components.

### Inspecting the calendar event

var fireDateComponents: DateComponents

The date components that specify when the event is triggered.

## Relationships

### Inherits From

- HMTimeEvent

### Inherited By

- HMMutableCalendarEvent

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

### Dates and times

class HMMutableCalendarEvent

A mutable event that fires at a specified time.

class HMTimeEvent

An abstract superclass for time-based events.

