

- Core Foundation
-  CFRunLoopObserverGetOrder(\_:) 

Function

# CFRunLoopObserverGetOrder(\_:)

Returns the ordering parameter for a CFRunLoopObserver object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopObserverGetOrder(_ observer: CFRunLoopObserver!) -> CFIndex
```

## Parameters 

`observer`  

The run loop observer to examine.

## Return Value

The ordering parameter for `observer`. When multiple observers are scheduled in the same run loop mode and stage, this value determines the order (from small to large) in which the observers are called.

## See Also

### CFRunLoopObserver Miscellaneous Functions

func CFRunLoopObserverCreateWithHandler(CFAllocator!, CFOptionFlags, Bool, CFIndex, ((CFRunLoopObserver?, CFRunLoopActivity) -> Void)!) -> CFRunLoopObserver!

Creates a CFRunLoopObserver object with a block-based handler.

func CFRunLoopObserverCreate(CFAllocator!, CFOptionFlags, Bool, CFIndex, CFRunLoopObserverCallBack!, UnsafeMutablePointer&lt;CFRunLoopObserverContext>!) -> CFRunLoopObserver!

Creates a CFRunLoopObserver object with a function callback.

func CFRunLoopObserverDoesRepeat(CFRunLoopObserver!) -> Bool

Returns a Boolean value that indicates whether a CFRunLoopObserver repeats.

func CFRunLoopObserverGetActivities(CFRunLoopObserver!) -> CFOptionFlags

Returns the run loop stages during which an observer runs.

func CFRunLoopObserverGetContext(CFRunLoopObserver!, UnsafeMutablePointer&lt;CFRunLoopObserverContext>!)

Returns the context information for a CFRunLoopObserver object.

func CFRunLoopObserverGetTypeID() -> CFTypeID

Returns the type identifier for the CFRunLoopObserver opaque type.

func CFRunLoopObserverInvalidate(CFRunLoopObserver!)

Invalidates a CFRunLoopObserver object, stopping it from ever firing again.

func CFRunLoopObserverIsValid(CFRunLoopObserver!) -> Bool

Returns a Boolean value that indicates whether a CFRunLoopObserver object is valid and able to fire.

