

- Core Foundation
-  CFRunLoopSourceSignal(\_:) 

Function

# CFRunLoopSourceSignal(\_:)

Signals a CFRunLoopSource object, marking it as ready to fire.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopSourceSignal(_ source: CFRunLoopSource!)
```

## Parameters 

`source`  

The run loop source to signal.

## Discussion

This function has no effect on version 1 sources, which are automatically handled when Mach messages arrive for them. After signaling a version 0 source, you need to call CFRunLoopWakeUp(_:) on one of the run loops in which the source is registered to get the source handled immediately.

## See Also

### CFRunLoopSource Miscellaneous Functions

func CFRunLoopSourceCreate(CFAllocator!, CFIndex, UnsafeMutablePointer&lt;CFRunLoopSourceContext>!) -> CFRunLoopSource!

Creates a CFRunLoopSource object.

func CFRunLoopSourceGetContext(CFRunLoopSource!, UnsafeMutablePointer&lt;CFRunLoopSourceContext>!)

Returns the context information for a CFRunLoopSource object.

func CFRunLoopSourceGetOrder(CFRunLoopSource!) -> CFIndex

Returns the ordering parameter for a CFRunLoopSource object.

func CFRunLoopSourceGetTypeID() -> CFTypeID

Returns the type identifier of the CFRunLoopSource opaque type.

func CFRunLoopSourceInvalidate(CFRunLoopSource!)

Invalidates a CFRunLoopSource object, stopping it from ever firing again.

func CFRunLoopSourceIsValid(CFRunLoopSource!) -> Bool

Returns a Boolean value that indicates whether a CFRunLoopSource object is valid and able to fire.

