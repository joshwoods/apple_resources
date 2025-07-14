

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IODelay 

Function

# IODelay

Spin delay for a number of microseconds.

macOS 10.0+

``` source
void IODelay(unsigned int microseconds);
```

## Parameters 

`microseconds`  

The integer number of microseconds to spin wait.

## Discussion

This function spins to delay for at least the number of specified microseconds. Since the CPU is busy spinning no time is made available to other processes; this method of delay should be used only for short periods. Also, the AbsoluteTime based APIs of kern/clock.h provide finer grained and lower cost delays.

## See Also

### Sleep

IOPause

Spin delay for a number of nanoseconds.

IOSleep

Sleep the calling thread for a number of milliseconds.

IOSleepWithLeeway

