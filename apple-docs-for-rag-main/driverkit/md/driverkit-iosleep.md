

- DriverKit
-  IOSleep 

Function

# IOSleep

Sleep the calling thread for a number of milliseconds.

DriverKitiOSiPadOSmacOS

``` source
void IOSleep(uint64_t ms);
```

## Parameters 

`ms`  

The integer number of milliseconds to wait.

## Discussion

This function blocks the calling thread for at least the number of specified milliseconds, giving time to other processes.

## See Also

### Thread Utilities

IODelay

Sleep the calling thread for a number of microseconds.

