

- DriverKit
-  mach_continuous_time 

Function

# mach_continuous_time

Returns current value of a clock that increments monotonically in tick units (starting at an arbitrary point), including while the system is asleep.

DriverKitiOSiPadOSmacOS

``` source
uint64_t mach_continuous_time();
```

## Return Value

Value of mach continous time clock.

## Discussion

Prefer to use the equivalent `clock_gettime_nsec_np(CLOCK_MONOTONIC_RAW)` in nanoseconds.

## See Also

### Mach Timebase

mach_absolute_time

Returns current value of a clock that increments monotonically in tick units (starting at an arbitrary point), this clock does not increment while the system is asleep.

mach_timebase_info

Returns fraction to multiply a value in mach tick units with to convert it to nanoseconds.

mach_timebase_info_t

Time Scales

