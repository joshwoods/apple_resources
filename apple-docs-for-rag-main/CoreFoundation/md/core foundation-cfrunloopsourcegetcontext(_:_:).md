

- Core Foundation
-  CFRunLoopSourceGetContext(\_:\_:) 

Function

# CFRunLoopSourceGetContext(\_:\_:)

Returns the context information for a CFRunLoopSource object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopSourceGetContext(
    _ source: CFRunLoopSource!,
    _ context: UnsafeMutablePointer!
)
```

## Parameters 

`source`  

The run loop source to examine.

`context`  

A pointer to the structure into which the context information for `source` is to be copied. The information being returned is the same information passed to CFRunLoopSourceCreate(_:_:_:) when creating `source`.

## Discussion

Run loop sources come in two versions with different-sized context structures. `context` must point to the correct version of the structure for `source`. Before calling this function, you need to initialize the `version` member of `context` with the version number (either 0 or 1) of `source`.

## See Also

### CFRunLoopSource Miscellaneous Functions

func CFRunLoopSourceCreate(CFAllocator!, CFIndex, UnsafeMutablePointer&lt;CFRunLoopSourceContext>!) -> CFRunLoopSource!

Creates a CFRunLoopSource object.

func CFRunLoopSourceGetOrder(CFRunLoopSource!) -> CFIndex

Returns the ordering parameter for a CFRunLoopSource object.

func CFRunLoopSourceGetTypeID() -> CFTypeID

Returns the type identifier of the CFRunLoopSource opaque type.

func CFRunLoopSourceInvalidate(CFRunLoopSource!)

Invalidates a CFRunLoopSource object, stopping it from ever firing again.

func CFRunLoopSourceIsValid(CFRunLoopSource!) -> Bool

Returns a Boolean value that indicates whether a CFRunLoopSource object is valid and able to fire.

func CFRunLoopSourceSignal(CFRunLoopSource!)

Signals a CFRunLoopSource object, marking it as ready to fire.

