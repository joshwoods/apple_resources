

- Dispatch
-  DispatchSourceTimer 

Protocol

# DispatchSourceTimer

A dispatch source that submits the event handler block based on a timer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol DispatchSourceTimer : DispatchSourceProtocol, Sendable
```

## Overview

You do not adopt this protocol in your objects. Instead, use the makeTimerSource(flags:queue:) method to create an object that adopts this protocol.

## Topics

### Scheduling the Timer Trigger Conditions

func schedule(deadline: DispatchTime, repeating: DispatchTimeInterval, leeway: DispatchTimeInterval)

Schedules a timer with the specified deadline, repeat interval, and leeway values.

func schedule(deadline: DispatchTime, repeating: Double, leeway: DispatchTimeInterval)

Schedules a timer with the specified deadline, repeat interval, and leeway values.

func schedule(wallDeadline: DispatchWallTime, repeating: DispatchTimeInterval, leeway: DispatchTimeInterval)

Schedules a timer with the specified time, repeat interval, and leeway values.

func schedule(wallDeadline: DispatchWallTime, repeating: Double, leeway: DispatchTimeInterval)

Schedules a timer with the specified time, repeat interval, and leeway values.

### Deprecated

func scheduleOneshot(deadline: DispatchTime, leeway: DispatchTimeInterval)

Schedules a timer to fire once with the specified deadline and leeway values.

Deprecated

func scheduleOneshot(wallDeadline: DispatchWallTime, leeway: DispatchTimeInterval)

Schedules a timer to fire once with the specified deadline and leeway values.

Deprecated

func scheduleRepeating(deadline: DispatchTime, interval: DispatchTimeInterval, leeway: DispatchTimeInterval)

Schedules a repeating timer with the specified deadline, repeat interval, and leeway values.

Deprecated

func scheduleRepeating(deadline: DispatchTime, interval: Double, leeway: DispatchTimeInterval)

Schedules a repeating timer with the specified deadline, repeat interval, and leeway values.

Deprecated

func scheduleRepeating(wallDeadline: DispatchWallTime, interval: Double, leeway: DispatchTimeInterval)

Schedules a repeating timer with the specified time, repeat interval, and leeway values.

Deprecated

func scheduleRepeating(wallDeadline: DispatchWallTime, interval: DispatchTimeInterval, leeway: DispatchTimeInterval)

Schedules a repeating timer with the specified time, repeat interval, and leeway values.

Deprecated

## Relationships

### Inherits From

- DispatchSourceProtocol
- NSObjectProtocol
- Sendable

### Conforming Types

- DispatchSource

## See Also

### Creating a Timer Source

class func makeTimerSource(flags: DispatchSource.TimerFlags, queue: DispatchQueue?) -> any DispatchSourceTimer

Creates a new dispatch source object for monitoring timer events.

struct TimerFlags

Flags to use when configuring a timer dispatch source.

