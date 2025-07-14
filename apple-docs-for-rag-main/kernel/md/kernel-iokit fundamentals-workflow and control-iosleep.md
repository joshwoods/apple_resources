

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOSleep 

Function

# IOSleep

Sleep the calling thread for a number of milliseconds.

macOS 10.0+

``` source
void IOSleep(unsigned int milliseconds);
```

## Parameters 

`milliseconds`  

The integer number of milliseconds to wait.

## Discussion

This function blocks the calling thread for at least the number of specified milliseconds, giving time to other processes.

## See Also

### Sleep

IODelay

Spin delay for a number of microseconds.

IOPause

Spin delay for a number of nanoseconds.

IOSleepWithLeeway

