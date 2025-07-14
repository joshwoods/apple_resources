

- Core Foundation
-  CFRunLoopObserverDoesRepeat(\_:) 

Function

# CFRunLoopObserverDoesRepeat(\_:)

Returns a Boolean value that indicates whether a CFRunLoopObserver repeats.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopObserverDoesRepeat(_ observer: CFRunLoopObserver!) -> Bool
```

## Parameters 

`observer`  

The run loop observer to examine.

## Return Value

`true` if `observer` is processed during every pass through the run loop; `false` if `observer` is processed once and then is invalidated.

## See Also

### CFRunLoopObserver Miscellaneous Functions

func CFRunLoopObserverCreateWithHandler(CFAllocator!, CFOptionFlags, Bool, CFIndex, ((CFRunLoopObserver?, CFRunLoopActivity) -> Void)!) -> CFRunLoopObserver!

Creates a CFRunLoopObserver object with a block-based handler.

func CFRunLoopObserverCreate(CFAllocator!, CFOptionFlags, Bool, CFIndex, CFRunLoopObserverCallBack!, UnsafeMutablePointer&lt;CFRunLoopObserverContext>!) -> CFRunLoopObserver!

Creates a CFRunLoopObserver object with a function callback.

func CFRunLoopObserverGetActivities(CFRunLoopObserver!) -> CFOptionFlags

Returns the run loop stages during which an observer runs.

func CFRunLoopObserverGetContext(CFRunLoopObserver!, UnsafeMutablePointer&lt;CFRunLoopObserverContext>!)

Returns the context information for a CFRunLoopObserver object.

func CFRunLoopObserverGetOrder(CFRunLoopObserver!) -> CFIndex

Returns the ordering parameter for a CFRunLoopObserver object.

func CFRunLoopObserverGetTypeID() -> CFTypeID

Returns the type identifier for the CFRunLoopObserver opaque type.

func CFRunLoopObserverInvalidate(CFRunLoopObserver!)

Invalidates a CFRunLoopObserver object, stopping it from ever firing again.

func CFRunLoopObserverIsValid(CFRunLoopObserver!) -> Bool

Returns a Boolean value that indicates whether a CFRunLoopObserver object is valid and able to fire.

