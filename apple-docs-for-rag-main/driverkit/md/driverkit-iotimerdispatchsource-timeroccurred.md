

- DriverKit
- IOTimerDispatchSource
-  TimerOccurred 

Instance Method

# TimerOccurred

Executes custom code when the timer fires.

DriverKitiOSiPadOSmacOS

``` source
void TimerOccurred(OSAction * action, uint64_t time);
```

## Parameters 

`action`  

The action object being executed.

`time`  

The actual time at which the timer fired. The system calls mach_absolute_time precisely when the timer fires and passes that value to this parameter.

## Discussion

Use this method as a prototype for declaring your own custom timer handlers. When declaring your method, use the TYPE macro to indicate that your method has the same parameters and return value as this method.

Use the implementation of your method to perform any custom actions related to the timer’s expiration.

## See Also

### Declaring Actions

CheckForWork

Checks for events to handle.

