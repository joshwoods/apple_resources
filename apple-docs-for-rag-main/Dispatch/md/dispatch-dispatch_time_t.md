

- Dispatch
-  dispatch_time_t 

Type Alias

# dispatch_time_t

An abstract representation of time.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias dispatch_time_t = UInt64
```

## Topics

### Well-Defined Times

var DISPATCH_TIME_NOW: UInt64

var DISPATCH_TIME_FOREVER: UInt64

### Time Multiplier Constants

var USEC_PER_SEC: UInt64

var NSEC_PER_SEC: UInt64

var NSEC_PER_MSEC: UInt64

var NSEC_PER_USEC: UInt64

## See Also

### Time Constructs

struct DispatchTime

A point in time relative to the default clock, with nanosecond precision.

struct DispatchWallTime

An absolute point in time according to the wall clock, with microsecond precision.

enum DispatchTimeInterval

A number of seconds, millisconds, microseconds, or nanoseconds.

enum DispatchTimeoutResult

A result value indicating whether a dispatch operation finished before a specified time.

var DISPATCH_WALLTIME_NOW: UInt

The current time.

Wall Time Constants

Constants for wall time values.

