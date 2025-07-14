

- DriverKit
-  mach_timebase_info_t 

Type Alias

# mach_timebase_info_t

DriverKitiOSiPadOSmacOS

``` source
typedef struct mach_timebase_info * mach_timebase_info_t;
```

## See Also

### Mach Timebase

mach_absolute_time

Returns current value of a clock that increments monotonically in tick units (starting at an arbitrary point), this clock does not increment while the system is asleep.

mach_continuous_time

Returns current value of a clock that increments monotonically in tick units (starting at an arbitrary point), including while the system is asleep.

mach_timebase_info

Returns fraction to multiply a value in mach tick units with to convert it to nanoseconds.

Time Scales

