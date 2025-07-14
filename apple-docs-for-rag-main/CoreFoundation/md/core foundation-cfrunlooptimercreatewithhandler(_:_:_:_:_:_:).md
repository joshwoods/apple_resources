

- Core Foundation
-  CFRunLoopTimerCreateWithHandler(\_:\_:\_:\_:\_:\_:) 

Function

# CFRunLoopTimerCreateWithHandler(\_:\_:\_:\_:\_:\_:)

Creates a new CFRunLoopTimer object with a block-based handler.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFRunLoopTimerCreateWithHandler(
    _ allocator: CFAllocator!,
    _ fireDate: CFAbsoluteTime,
    _ interval: CFTimeInterval,
    _ flags: CFOptionFlags,
    _ order: CFIndex,
    _ block: ((CFRunLoopTimer?) -> Void)!
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

`block`  

The block invoked when the timer fires. The block takes one argument:

`timer`  
The run loop timer that is firing.

## Return Value

The new CFRunLoopTimer object. Ownership follows the Create Rule described in Ownership Policy.

## Discussion

A timer needs to be added to a run loop mode before it will fire. To add the timer to a run loop, use CFRunLoopAddTimer(_:_:_:). A timer can be registered to only one run loop at a time, although it can be in multiple modes within that run loop.

## See Also

### CFRunLoopTimer Miscellaneous Functions

func CFRunLoopTimerCreate(CFAllocator!, CFAbsoluteTime, CFTimeInterval, CFOptionFlags, CFIndex, CFRunLoopTimerCallBack!, UnsafeMutablePointer&lt;CFRunLoopTimerContext>!) -> CFRunLoopTimer!

Creates a new CFRunLoopTimer object with a function callback.

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

