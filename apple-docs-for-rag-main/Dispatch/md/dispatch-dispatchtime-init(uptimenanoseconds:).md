

- Dispatch
- DispatchTime
-  init(uptimeNanoseconds:) 

Initializer

# init(uptimeNanoseconds:)

Creates a time relative to the amount of time the system has been running.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(uptimeNanoseconds: UInt64)
```

## Parameters 

`uptimeNanoseconds`  

The number of nanoseconds since boot, excluding any time the system spent asleep.

## Discussion

On Apple platforms, this clock is the same as the value returned by mach_absolute_time when converted into nanoseconds.

