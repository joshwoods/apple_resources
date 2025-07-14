

- Core Foundation
-  CFRunLoopTimerGetContext(\_:\_:) 

Function

# CFRunLoopTimerGetContext(\_:\_:)

Returns the context information for a CFRunLoopTimer object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopTimerGetContext(
    _ timer: CFRunLoopTimer!,
    _ context: UnsafeMutablePointer!
)
```

## Parameters 

`timer`  

The run loop timer to examine.

`context`  

A pointer to the structure into which the context information for `timer` is to be copied. The information being returned is the same information passed to CFRunLoopTimerCreate(_:_:_:_:_:_:_:) when creating `timer`.

## Discussion

The context version number for run loop timers is currently 0. Before calling this function, you need to initialize the `version` member of `context` to `0`.

## See Also

### CFRunLoopTimer Miscellaneous Functions

func CFRunLoopTimerCreateWithHandler(CFAllocator!, CFAbsoluteTime, CFTimeInterval, CFOptionFlags, CFIndex, ((CFRunLoopTimer?) -> Void)!) -> CFRunLoopTimer!

Creates a new CFRunLoopTimer object with a block-based handler.

func CFRunLoopTimerCreate(CFAllocator!, CFAbsoluteTime, CFTimeInterval, CFOptionFlags, CFIndex, CFRunLoopTimerCallBack!, UnsafeMutablePointer&lt;CFRunLoopTimerContext>!) -> CFRunLoopTimer!

Creates a new CFRunLoopTimer object with a function callback.

func CFRunLoopTimerDoesRepeat(CFRunLoopTimer!) -> Bool

Returns a Boolean value that indicates whether a CFRunLoopTimer object repeats.

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

