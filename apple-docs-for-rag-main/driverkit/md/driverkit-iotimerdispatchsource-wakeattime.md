

- DriverKit
- IOTimerDispatchSource
-  WakeAtTime 

Instance Method

# WakeAtTime

Schedules a callback from the timer.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t WakeAtTime(uint64_t options, uint64_t deadline, uint64_t leeway);
```

## Parameters 

`options`  

The timebase to use when interpreting the `deadline` and `leeway` parameters. For a list of possible values, see Clock Types.

`deadline`  

The time at which to execute your action. The meaning of this parameter depends on the timebase you specified in the `options` parameter.

`leeway`  

The maximum amount of time beyond the scheduled `deadline` that the system may wait before executing your action. Leeway values improve the system’s power usage by letting the system schedule timers at a more advantageous time. The system guarantees the execution of the timer’s action before the combined `deadline` and `leeway` values expire.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Use this method to schedule the execution time for your timer. Call this method from a block running on the same dispatch queue you passed to the Create method. If a previously scheduled timer has not yet fired, calling this method replaces the old time with the new value.

## See Also

### Rescheduling the Timer

Clock Types

Clock types to use when configuring a timer.

