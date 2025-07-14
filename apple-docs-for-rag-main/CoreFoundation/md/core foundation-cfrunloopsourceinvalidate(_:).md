

- Core Foundation
-  CFRunLoopSourceInvalidate(\_:) 

Function

# CFRunLoopSourceInvalidate(\_:)

Invalidates a CFRunLoopSource object, stopping it from ever firing again.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopSourceInvalidate(_ source: CFRunLoopSource!)
```

## Parameters 

`source`  

The run loop source to invalidate.

## Discussion

Once invalidated, `source` will never fire and call its perform callback function again. This function automatically removes `source` from all the run loop modes in which it was registered. If `source` is a version 0 source, this function calls its `cancel` callback function as it is removed from each run loop mode. The memory for `source` is not deallocated unless the run loop held the only reference to `source`.

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

func CFRunLoopSourceIsValid(CFRunLoopSource!) -> Bool

Returns a Boolean value that indicates whether a CFRunLoopSource object is valid and able to fire.

func CFRunLoopSourceSignal(CFRunLoopSource!)

Signals a CFRunLoopSource object, marking it as ready to fire.

