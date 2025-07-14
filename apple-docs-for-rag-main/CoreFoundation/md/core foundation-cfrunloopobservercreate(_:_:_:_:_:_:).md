

- Core Foundation
-  CFRunLoopObserverCreate(\_:\_:\_:\_:\_:\_:) 

Function

# CFRunLoopObserverCreate(\_:\_:\_:\_:\_:\_:)

Creates a CFRunLoopObserver object with a function callback.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopObserverCreate(
    _ allocator: CFAllocator!,
    _ activities: CFOptionFlags,
    _ repeats: Bool,
    _ order: CFIndex,
    _ callout: CFRunLoopObserverCallBack!,
    _ context: UnsafeMutablePointer!
) -> CFRunLoopObserver!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`activities`  

Set of flags identifying the activity stages of the run loop during which the observer should be called. See CFRunLoopActivityfor the list of stages. To have the observer called at multiple stages in the run loop, combine the CFRunLoopActivity values using the bitwise-OR operator.

`repeats`  

A flag identifying whether the observer should be called only once or every time through the run loop. If `repeats` is `false`, the observer is invalidated after it is called once, even if the observer was scheduled to be called at multiple stages within the run loop.

`order`  

A priority index indicating the order in which run loop observers are processed. When multiple run loop observers are scheduled in the same activity stage in a given run loop mode, the observers are processed in increasing order of this parameter. Pass 0 unless there is a reason to do otherwise.

`callout`  

The callback function invoked when the observer runs.

`context`  

A structure holding contextual information for the run loop observer. The function copies the information out of the structure, so the memory pointed to by `context` does not need to persist beyond the function call. Can be `NULL` if the observer does not need the context’s `info` pointer to keep track of state.

## Return Value

The new CFRunLoopObserver object. Ownership follows the Create Rule described in Ownership Policy.

## Discussion

The run loop observer is not automatically added to a run loop. To add the observer to a run loop, use CFRunLoopAddObserver(_:_:_:). An observer can be registered to only one run loop, although it can be added to multiple run loop modes within that run loop.

## See Also

### CFRunLoopObserver Miscellaneous Functions

func CFRunLoopObserverCreateWithHandler(CFAllocator!, CFOptionFlags, Bool, CFIndex, ((CFRunLoopObserver?, CFRunLoopActivity) -> Void)!) -> CFRunLoopObserver!

Creates a CFRunLoopObserver object with a block-based handler.

func CFRunLoopObserverDoesRepeat(CFRunLoopObserver!) -> Bool

Returns a Boolean value that indicates whether a CFRunLoopObserver repeats.

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

