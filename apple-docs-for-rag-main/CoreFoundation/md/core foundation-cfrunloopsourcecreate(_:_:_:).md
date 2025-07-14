

- Core Foundation
-  CFRunLoopSourceCreate(\_:\_:\_:) 

Function

# CFRunLoopSourceCreate(\_:\_:\_:)

Creates a CFRunLoopSource object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopSourceCreate(
    _ allocator: CFAllocator!,
    _ order: CFIndex,
    _ context: UnsafeMutablePointer!
) -> CFRunLoopSource!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`order`  

A priority index indicating the order in which run loop sources are processed. When multiple run loop sources are firing in a single pass through the run loop, the sources are processed in increasing order of this parameter. If the run loop is set to process only one source per loop, only the highest priority source, the one with the lowest `order` value, is processed. This value is ignored for version 1 sources. Pass 0 unless there is a reason to do otherwise.

`context`  

A structure holding contextual information for the run loop source. The function copies the information out of the structure, so the memory pointed to by `context` does not need to persist beyond the function call.

## Return Value

The new CFRunLoopSource object. You are responsible for releasing this object.

## Discussion

The run loop source is not automatically added to a run loop. Ownership follows the The Create Rule.

## See Also

### CFRunLoopSource Miscellaneous Functions

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

func CFRunLoopSourceSignal(CFRunLoopSource!)

Signals a CFRunLoopSource object, marking it as ready to fire.

