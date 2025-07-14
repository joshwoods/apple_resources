

- Core Foundation
-  CFMachPortSetInvalidationCallBack(\_:\_:) 

Function

# CFMachPortSetInvalidationCallBack(\_:\_:)

Sets the callback function invoked when a CFMachPort object is invalidated.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMachPortSetInvalidationCallBack(
    _ port: CFMachPort!,
    _ callout: CFMachPortInvalidationCallBack!
)
```

## Parameters 

`port`  

The CFMachPort object to modify.

`callout`  

The callback function to invoke when `port` is invalidated. Pass `NULL` to remove a callback.

## Discussion

If `port` is already invalid, `callout` is invoked immediately.

## See Also

### Configuring a CFMachPort Object

func CFMachPortInvalidate(CFMachPort!)

Invalidates a CFMachPort object, stopping it from receiving any more messages.

func CFMachPortCreateRunLoopSource(CFAllocator!, CFMachPort!, CFIndex) -> CFRunLoopSource!

Creates a CFRunLoopSource object for a CFMachPort object.

