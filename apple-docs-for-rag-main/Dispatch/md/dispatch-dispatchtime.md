

- Dispatch
-  DispatchTime 

Structure

# DispatchTime

A point in time relative to the default clock, with nanosecond precision.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct DispatchTime
```

## Overview

On Apple platforms, the default clock is based on the Mach absolute time unit.

## Topics

### Getting Well-Known Times

static func now() -> DispatchTime

Returns the current time.

static let distantFuture: DispatchTime

A time in the distant future.

### Creating a Dispatch Time Object

init(uptimeNanoseconds: UInt64)

Creates a time relative to the amount of time the system has been running.

### Getting the Time

let rawValue: dispatch_time_t

Returns the underlying time value.

var uptimeNanoseconds: UInt64

Returns the number of nanoseconds since boot, excluding any time the system spent asleep.

### Modifying the Value

func advanced(by: DispatchTimeInterval) -> DispatchTime

func distance(to: DispatchTime) -> DispatchTimeInterval

### Operator Functions

func + (DispatchTime, Double) -> DispatchTime

func + (DispatchTime, DispatchTimeInterval) -> DispatchTime

func - (DispatchTime, Double) -> DispatchTime

func - (DispatchTime, DispatchTimeInterval) -> DispatchTime

## Relationships

### Conforms To

- Comparable
- Equatable
- Sendable

## See Also

### Time Constructs

struct DispatchWallTime

An absolute point in time according to the wall clock, with microsecond precision.

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

