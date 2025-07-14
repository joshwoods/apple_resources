

- Core Foundation
-  CFRunLoopObserverGetContext(\_:\_:) 

Function

# CFRunLoopObserverGetContext(\_:\_:)

Returns the context information for a CFRunLoopObserver object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopObserverGetContext(
    _ observer: CFRunLoopObserver!,
    _ context: UnsafeMutablePointer!
)
```

## Parameters 

`observer`  

The run loop observer to examine.

`context`  

Upon return, contains the context information for `observer`. This is the same information passed to CFRunLoopObserverCreate(_:_:_:_:_:_:) when creating `observer`.

## Discussion

The context version number for run loop observers is currently `0`. Before calling this function, you need to initialize the `version` member of `context` to `0`.

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

func CFRunLoopObserverGetOrder(CFRunLoopObserver!) -> CFIndex

Returns the ordering parameter for a CFRunLoopObserver object.

func CFRunLoopObserverGetTypeID() -> CFTypeID

Returns the type identifier for the CFRunLoopObserver opaque type.

func CFRunLoopObserverInvalidate(CFRunLoopObserver!)

Invalidates a CFRunLoopObserver object, stopping it from ever firing again.

func CFRunLoopObserverIsValid(CFRunLoopObserver!) -> Bool

Returns a Boolean value that indicates whether a CFRunLoopObserver object is valid and able to fire.

