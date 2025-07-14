

- Core Foundation
-  CFRunLoopSourceGetTypeID() 

Function

# CFRunLoopSourceGetTypeID()

Returns the type identifier of the CFRunLoopSource opaque type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopSourceGetTypeID() -> CFTypeID
```

## Return Value

The type identifier for the CFRunLoopSource opaque type.

## See Also

### CFRunLoopSource Miscellaneous Functions

func CFRunLoopSourceCreate(CFAllocator!, CFIndex, UnsafeMutablePointer&lt;CFRunLoopSourceContext>!) -> CFRunLoopSource!

Creates a CFRunLoopSource object.

func CFRunLoopSourceGetContext(CFRunLoopSource!, UnsafeMutablePointer&lt;CFRunLoopSourceContext>!)

Returns the context information for a CFRunLoopSource object.

func CFRunLoopSourceGetOrder(CFRunLoopSource!) -> CFIndex

Returns the ordering parameter for a CFRunLoopSource object.

func CFRunLoopSourceInvalidate(CFRunLoopSource!)

Invalidates a CFRunLoopSource object, stopping it from ever firing again.

func CFRunLoopSourceIsValid(CFRunLoopSource!) -> Bool

Returns a Boolean value that indicates whether a CFRunLoopSource object is valid and able to fire.

func CFRunLoopSourceSignal(CFRunLoopSource!)

Signals a CFRunLoopSource object, marking it as ready to fire.

