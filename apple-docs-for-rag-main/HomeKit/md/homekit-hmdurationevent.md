

- HomeKit
-  HMDurationEvent 

Class

# HMDurationEvent

An event that ends after the specified time duration.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class HMDurationEvent
```

## Overview

Use a duration event to specify that a different event should end after a period of time.

## Topics

### Creating a duration event

init(duration: TimeInterval)

Creates a duration event with the specified time duration.

### Inspecting a duration event

var duration: TimeInterval

The event’s duration, in seconds.

## Relationships

### Inherits From

- HMTimeEvent

### Inherited By

- HMMutableDurationEvent

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

### Durations

class HMMutableDurationEvent

A mutable event that fires after the specified time duration.

