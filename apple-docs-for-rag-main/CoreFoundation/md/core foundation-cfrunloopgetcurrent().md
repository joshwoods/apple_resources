

- Core Foundation
-  CFRunLoopGetCurrent() 

Function

# CFRunLoopGetCurrent()

Returns the CFRunLoop object for the current thread.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopGetCurrent() -> CFRunLoop!
```

## Return Value

Current thread’s run loop. Ownership follows the The Get Rule.

## Discussion

Each thread has exactly one run loop associated with it.

## See Also

### Related Documentation

Threading Programming Guide

Concurrency Programming Guide

### Getting a Run Loop

func CFRunLoopGetMain() -> CFRunLoop!

Returns the main CFRunLoop object.

