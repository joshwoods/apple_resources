

- Core Foundation
-  CFRunLoopSourceGetOrder(\_:) 

Function

# CFRunLoopSourceGetOrder(\_:)

Returns the ordering parameter for a CFRunLoopSource object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopSourceGetOrder(_ source: CFRunLoopSource!) -> CFIndex
```

## Parameters 

`source`  

The run loop source to examine.

## Return Value

The ordering parameter for `source`, which the run loop uses (for version 0 sources only) to determine the order in which sources are processed when multiple sources are firing.

## See Also

### CFRunLoopSource Miscellaneous Functions

func CFRunLoopSourceCreate(CFAllocator!, CFIndex, UnsafeMutablePointer&lt;CFRunLoopSourceContext>!) -> CFRunLoopSource!

Creates a CFRunLoopSource object.

func CFRunLoopSourceGetContext(CFRunLoopSource!, UnsafeMutablePointer&lt;CFRunLoopSourceContext>!)

Returns the context information for a CFRunLoopSource object.

func CFRunLoopSourceGetTypeID() -> CFTypeID

Returns the type identifier of the CFRunLoopSource opaque type.

func CFRunLoopSourceInvalidate(CFRunLoopSource!)

Invalidates a CFRunLoopSource object, stopping it from ever firing again.

func CFRunLoopSourceIsValid(CFRunLoopSource!) -> Bool

Returns a Boolean value that indicates whether a CFRunLoopSource object is valid and able to fire.

func CFRunLoopSourceSignal(CFRunLoopSource!)

Signals a CFRunLoopSource object, marking it as ready to fire.

