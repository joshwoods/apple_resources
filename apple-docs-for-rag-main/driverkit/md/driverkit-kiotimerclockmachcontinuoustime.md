

- DriverKit
-  kIOTimerClockMachContinuousTime 

Enumeration Case

# kIOTimerClockMachContinuousTime

A clock type representing the number of ticks since the last reboot, including when the computer is asleep.

DriverKitiOSiPadOSmacOS

``` source
kIOTimerClockMachContinuousTime
```

## Discussion

This constant is a clock type whose value is from `mach_continuous_time()` in tick units.

## See Also

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

