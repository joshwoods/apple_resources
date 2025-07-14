

- Core Foundation
-  CFRunLoopTimerGetInterval(\_:) 

Function

# CFRunLoopTimerGetInterval(\_:)

Returns the firing interval of a repeating CFRunLoopTimer object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopTimerGetInterval(_ timer: CFRunLoopTimer!) -> CFTimeInterval
```

## Parameters 

`timer`  

The run loop timer to examine.

## Return Value

The firing interval of `timer`. Returns `0` if `timer` does not repeat.

## See Also

### CFRunLoopTimer Miscellaneous Functions

func CFRunLoopTimerCreateWithHandler(CFAllocator!, CFAbsoluteTime, CFTimeInterval, CFOptionFlags, CFIndex, ((CFRunLoopTimer?) -> Void)!) -> CFRunLoopTimer!

Creates a new CFRunLoopTimer object with a block-based handler.

func CFRunLoopTimerCreate(CFAllocator!, CFAbsoluteTime, CFTimeInterval, CFOptionFlags, CFIndex, CFRunLoopTimerCallBack!, UnsafeMutablePointer&lt;CFRunLoopTimerContext>!) -> CFRunLoopTimer!

Creates a new CFRunLoopTimer object with a function callback.

func CFRunLoopTimerDoesRepeat(CFRunLoopTimer!) -> Bool

Returns a Boolean value that indicates whether a CFRunLoopTimer object repeats.

func CFRunLoopTimerGetContext(CFRunLoopTimer!, UnsafeMutablePointer&lt;CFRunLoopTimerContext>!)

Returns the context information for a CFRunLoopTimer object.

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

