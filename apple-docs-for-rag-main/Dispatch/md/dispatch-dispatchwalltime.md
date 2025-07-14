

- Dispatch
-  DispatchWallTime 

Structure

# DispatchWallTime

An absolute point in time according to the wall clock, with microsecond precision.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct DispatchWallTime
```

## Topics

### Getting Well-Known Times

static func now() -> DispatchWallTime

Returns the current time.

static let distantFuture: DispatchWallTime

A time in the distant future.

### Creating a Dispatch Wall Time Object

init(timespec: timespec)

Creates an absolute time for a specified value.

### Getting the Time

let rawValue: dispatch_time_t

The underlying time value.

### Operator Functions

func + (DispatchWallTime, DispatchTimeInterval) -> DispatchWallTime

func + (DispatchWallTime, Double) -> DispatchWallTime

func - (DispatchWallTime, Double) -> DispatchWallTime

func - (DispatchWallTime, DispatchTimeInterval) -> DispatchWallTime

## Relationships

### Conforms To

- Comparable
- Equatable
- Sendable

## See Also

### Time Constructs

struct DispatchTime

A point in time relative to the default clock, with nanosecond precision.

enum DispatchTimeInterval

A number of seconds, millisconds, microseconds, or nanoseconds.

enum DispatchTimeoutResult

A result value indicating whether a dispatch operation finished before a specified time.

typealias dispatch_time_t

An abstract representation of time.

var DISPATCH_WALLTIME_NOW: UInt

The current time.

Wall Time Constants

Constants for wall time values.

