

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOPause 

Function

# IOPause

Spin delay for a number of nanoseconds.

macOS 10.5+

``` source
void IOPause(unsigned int nanoseconds);
```

## Parameters 

`microseconds`  

The integer number of nanoseconds to spin wait.

## Discussion

This function spins to delay for at least the number of specified nanoseconds. Since the CPU is busy spinning no time is made available to other processes; this method of delay should be used only for short periods.

## See Also

### Sleep

IODelay

Spin delay for a number of microseconds.

IOSleep

Sleep the calling thread for a number of milliseconds.

IOSleepWithLeeway

