

- HomeKit
-  HMSignificantTimeEvent 

Class

# HMSignificantTimeEvent

An event that fires at a time offset from a significant time-based event.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class HMSignificantTimeEvent
```

## Overview

Use this class to represent an event that fires at a time relative to a significant event, for example “30 minutes before sunset”.

## Topics

### Creating a significant time event

init(significantEvent: HMSignificantEvent, offset: DateComponents?)

Creates a new significant time event with the specified significant event and offset.

### Inspecting a significant time event

var significantEvent: HMSignificantEvent

The significant time-based event that is used to calculate when the event fires.

var offset: DateComponents?

The offset from the significant event that the event fires at.

## Relationships

### Inherits From

- HMTimeEvent

### Inherited By

- HMMutableSignificantTimeEvent

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

class HMMutableSignificantTimeEvent

A mutable event that fires at the specified temporal offset to a significant event.

