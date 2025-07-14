

- CarPlay
-  CPNowPlayingSportsClock 

Class

# CPNowPlayingSportsClock

A representation of the amount of time elapsed so far in this event, for events where the clock counts UP.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+

``` source
class CPNowPlayingSportsClock
```

## Overview

Or, a representation of the amount of time remaining in the event, or a section of the event (period/quarter/etc.) for events where the clock counts DOWN.

## Topics

### Initializers

init(elapsedTime: TimeInterval, paused: Bool)

Represents a duration of time that has elapsed so far in this event, or play period of the event (quarter/inning/period).

init(timeRemaining: TimeInterval, paused: Bool)

Represents an amount of time remaining in the event, or play period of the event (quarter/inning/period).

### Instance Properties

var countsUp: Bool

If true, the timer is counting UP, so as to indicate an amount of time elapsed so far in this event.

var isPaused: Bool

Whether the clock should be paused, e.g. due to a stoppage in play.

var timeValue: TimeInterval

The time value in the clock; either elapsed time or time remaining.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

