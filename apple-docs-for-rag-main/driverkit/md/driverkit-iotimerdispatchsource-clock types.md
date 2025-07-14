

- DriverKit
- IOTimerDispatchSource
-  Clock Types 

API Collection

# Clock Types

Clock types to use when configuring a timer.

## Topics

### Timer Options

kIOTimerClockUptimeRaw

A clock type that increments monotonically, but does not increment when the system is asleep.

kIOTimerClockMonotonicRaw

A clock type that increments monotonically, and is unaffected by frequency or time adjustmets.

kIOTimerClockRealTime

The system’s real time, expressed as the amount of time since the Epoch.

kIOTimerClockWallTime

The system’s wall-clock time, expressed as the amount of time since the Epoch.

kIOTimerClockMachAbsoluteTime

A clock type representing the numer of ticks since the last reboot.

kIOTimerClockMachContinuousTime

A clock type representing the number of ticks since the last reboot, including when the computer is asleep.

## See Also

### Rescheduling the Timer

WakeAtTime

Schedules a callback from the timer.

