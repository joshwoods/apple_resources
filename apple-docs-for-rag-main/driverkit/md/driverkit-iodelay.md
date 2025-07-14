

- DriverKit
-  IODelay 

Function

# IODelay

Sleep the calling thread for a number of microseconds.

DriverKitiOSiPadOSmacOS

``` source
void IODelay(uint64_t us);
```

## Parameters 

`us`  

The integer number of microseconds to wait.

## Discussion

This function blocks the calling thread for at least the number of specified microseconds, giving time to other processes.

## See Also

### Thread Utilities

IOSleep

Sleep the calling thread for a number of milliseconds.

