

- Dispatch
-  DispatchTimeInterval 

Enumeration

# DispatchTimeInterval

A number of seconds, millisconds, microseconds, or nanoseconds.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum DispatchTimeInterval
```

## Overview

Use DispatchTimeInterval values to specify the interval at which a DispatchSourceTimer fires or I/O handlers are invoked for a DispatchIO channel, as well as to increment and decrement DispatchTime values.

## Topics

### Enumeration Cases

case seconds(Int)

A number of seconds.

case milliseconds(Int)

A number of milliseconds.

case microseconds(Int)

A number of microseconds.

case nanoseconds(Int)

A number of nanoseconds.

case never

No interval.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Time Constructs

struct DispatchTime

A point in time relative to the default clock, with nanosecond precision.

struct DispatchWallTime

An absolute point in time according to the wall clock, with microsecond precision.

enum DispatchTimeoutResult

A result value indicating whether a dispatch operation finished before a specified time.

typealias dispatch_time_t

An abstract representation of time.

var DISPATCH_WALLTIME_NOW: UInt

The current time.

Wall Time Constants

Constants for wall time values.

