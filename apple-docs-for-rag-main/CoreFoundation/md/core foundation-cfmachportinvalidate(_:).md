

- Core Foundation
-  CFMachPortInvalidate(\_:) 

Function

# CFMachPortInvalidate(\_:)

Invalidates a CFMachPort object, stopping it from receiving any more messages.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMachPortInvalidate(_ port: CFMachPort!)
```

## Parameters 

`port`  

The CFMachPort object to invalidate.

## Discussion

Invalidating a CFMachPort object prevents the port from ever receiving any more messages. The CFMachPort object is not deallocated, though. If the port has not already been invalidated, the port’s invalidation callback function is invoked, if one has been set with CFMachPortSetInvalidationCallBack(_:_:). The CFMachPortContext `info` information for `port` is also released, if a release callback was specified in the port’s context structure. Finally, if a run loop source was created for `port`, the run loop source is invalidated, as well.

If the underlying Mach port is destroyed, the CFMachPort object is automatically invalidated.

## See Also

### Configuring a CFMachPort Object

func CFMachPortCreateRunLoopSource(CFAllocator!, CFMachPort!, CFIndex) -> CFRunLoopSource!

Creates a CFRunLoopSource object for a CFMachPort object.

func CFMachPortSetInvalidationCallBack(CFMachPort!, CFMachPortInvalidationCallBack!)

Sets the callback function invoked when a CFMachPort object is invalidated.

