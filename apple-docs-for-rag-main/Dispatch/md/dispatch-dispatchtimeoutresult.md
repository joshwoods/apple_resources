

- Dispatch
-  DispatchTimeoutResult 

Enumeration

# DispatchTimeoutResult

A result value indicating whether a dispatch operation finished before a specified time.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
@frozen
enum DispatchTimeoutResult
```

## Topics

### Enumeration Cases

case success

Indicates that a dispatch operation successfully finished before the specified time elapsed.

case timedOut

Indicates that a dispatch operation failed to finish before the specified time elapsed.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Time Constructs

struct DispatchTime

A point in time relative to the default clock, with nanosecond precision.

struct DispatchWallTime

An absolute point in time according to the wall clock, with microsecond precision.

enum DispatchTimeInterval

A number of seconds, millisconds, microseconds, or nanoseconds.

typealias dispatch_time_t

An abstract representation of time.

var DISPATCH_WALLTIME_NOW: UInt

The current time.

Wall Time Constants

Constants for wall time values.

