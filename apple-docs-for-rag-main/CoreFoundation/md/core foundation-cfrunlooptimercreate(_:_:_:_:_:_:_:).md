

- Core Foundation
-  CFRunLoopTimerCreate(\_:\_:\_:\_:\_:\_:\_:) 

Function

# CFRunLoopTimerCreate(\_:\_:\_:\_:\_:\_:\_:)

Creates a new CFRunLoopTimer object with a function callback.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopTimerCreate(
    _ allocator: CFAllocator!,
    _ fireDate: CFAbsoluteTime,
    _ interval: CFTimeInterval,
    _ flags: CFOptionFlags,
    _ order: CFIndex,
    _ callout: CFRunLoopTimerCallBack!,
    _ context: UnsafeMutablePointer!
) -> CFRunLoopTimer!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`fireDate`  

The time at which the timer should first fire. The fine precision (sub-millisecond at most) of the fire date may be adjusted slightly by the timer if there are implementation reasons to do so.

`interval`  

The firing interval of the timer. If `0` or negative, the timer fires once and then is automatically invalidated. The fine precision (sub-millisecond at most) of the interval may be adjusted slightly by the timer if implementation reasons to do so exist.

`flags`  

Currently ignored. Pass `0` for future compatibility.

`order`  

A priority index indicating the order in which run loop timers are processed. Run loop timers currently ignore this parameter. Pass `0`.

`callout`  

The callback function that is called when the timer fires.

`context`  

A structure holding contextual information for the run loop timer. The function copies the information out of the structure, so the memory pointed to by `context` does not need to persist beyond the function call. Can be `NULL` if the callback function does not need the context’s `info` pointer to keep track of state.

## Return Value

The new CFRunLoopTimer object. Ownership follows the The Create Rule.

## Discussion

A timer needs to be added to a run loop mode before it will fire. To add the timer to a run loop, use CFRunLoopAddTimer(_:_:_:). A timer can be registered to only one run loop at a time, although it can be in multiple modes within that run loop.

## See Also

### CFRunLoopTimer Miscellaneous Functions

func CFRunLoopTimerCreateWithHandler(CFAllocator!, CFAbsoluteTime, CFTimeInterval, CFOptionFlags, CFIndex, ((CFRunLoopTimer?) -> Void)!) -> CFRunLoopTimer!

Creates a new CFRunLoopTimer object with a block-based handler.

func CFRunLoopTimerDoesRepeat(CFRunLoopTimer!) -> Bool

Returns a Boolean value that indicates whether a CFRunLoopTimer object repeats.

func CFRunLoopTimerGetContext(CFRunLoopTimer!, UnsafeMutablePointer&lt;CFRunLoopTimerContext>!)

Returns the context information for a CFRunLoopTimer object.

func CFRunLoopTimerGetInterval(CFRunLoopTimer!) -> CFTimeInterval

Returns the firing interval of a repeating CFRunLoopTimer object.

func CFRunLoopTimerGetNextFireDate(CFRunLoopTimer!) -> CFAbsoluteTime

Returns the next firing time for a CFRunLoopTimer object.

func CFRunLoopTimerGetOrder(CFRunLoopTimer!) -> CFIndex

Returns the ordering parameter for a CFRunLoopTimer object.

func CFRunLoopTimerGetTypeID() -> CFTypeID

Returns the type identifier of the CFRunLoopTimer opaque type.

func CFRunLoopTimerInvalidate(CFRunLoopTimer!)

Invalidates a CFRunLoopTimer object, stopping it from ever firing again.

func CFRunLoopTimerIsValid(CFRunLoopTimer!) -> Bool

Returns a Boolean value that indicates whether a CFRunLoopTimer object is valid and able to fire.

func CFRunLoopTimerSetNextFireDate(CFRunLoopTimer!, CFAbsoluteTime)

Sets the next firing date for a CFRunLoopTimer object .

