

- Core Foundation
-  CFRunLoopObserverCreateWithHandler(\_:\_:\_:\_:\_:) 

Function

# CFRunLoopObserverCreateWithHandler(\_:\_:\_:\_:\_:)

Creates a CFRunLoopObserver object with a block-based handler.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFRunLoopObserverCreateWithHandler(
    _ allocator: CFAllocator!,
    _ activities: CFOptionFlags,
    _ repeats: Bool,
    _ order: CFIndex,
    _ block: ((CFRunLoopObserver?, CFRunLoopActivity) -> Void)!
) -> CFRunLoopObserver!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`activities`  

Set of flags identifying the activity stages of the run loop during which the observer is called. See CFRunLoopActivityfor the list of stages. To have the observer called at multiple stages in the run loop, combine the CFRunLoopActivity values using the bitwise-OR operator.

`repeats`  

A flag identifying whether the observer is called only once or every time through the run loop. If `repeats` is `false`, the observer is invalidated after it is called once, even if the observer was scheduled to be called at multiple stages within the run loop.

`order`  

A priority index indicating the order in which run loop observers are processed. When multiple run loop observers are scheduled in the same activity stage in a given run loop mode, the observers are processed in increasing order of this parameter. Pass 0 unless there is a reason to do otherwise.

`block`  

The block invoked when the observer runs. The block takes two arguments:

`observer`  
The run loop observer that is firing.

`activity`  
The current activity stage of the run loop.

## Return Value

The new CFRunLoopObserver object. Ownership follows the Create Rule described in Ownership Policy.

## Discussion

The run loop observer is not automatically added to a run loop. To add the observer to a run loop, use CFRunLoopAddObserver(_:_:_:). An observer can be registered to only one run loop, although it can be added to multiple run loop modes within that run loop.

## See Also

### CFRunLoopObserver Miscellaneous Functions

func CFRunLoopObserverCreate(CFAllocator!, CFOptionFlags, Bool, CFIndex, CFRunLoopObserverCallBack!, UnsafeMutablePointer&lt;CFRunLoopObserverContext>!) -> CFRunLoopObserver!

Creates a CFRunLoopObserver object with a function callback.

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

