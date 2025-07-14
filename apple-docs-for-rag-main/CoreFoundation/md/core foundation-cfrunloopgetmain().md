

- Core Foundation
-  CFRunLoopGetMain() 

Function

# CFRunLoopGetMain()

Returns the main CFRunLoop object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopGetMain() -> CFRunLoop!
```

## Return Value

The main run loop. Ownership follows the The Get Rule.

## See Also

### Getting a Run Loop

func CFRunLoopGetCurrent() -> CFRunLoop!

Returns the CFRunLoop object for the current thread.

