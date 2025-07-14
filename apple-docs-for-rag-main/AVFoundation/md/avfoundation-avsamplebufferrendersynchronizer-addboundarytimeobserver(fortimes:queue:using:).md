

- AVFoundation
- AVSampleBufferRenderSynchronizer
-  addBoundaryTimeObserver(forTimes:queue:using:) 

Instance Method

# addBoundaryTimeObserver(forTimes:queue:using:)

Requests invocation of a block when specified times are traversed during normal rendering.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func addBoundaryTimeObserver(
    forTimes times: [NSValue],
    queue: dispatch_queue_t?,
    using block: @escaping () -> Void
) -> Any
```

## Parameters 

`times`  

An array containing the times for which the observer requests notification.

`queue`  

The serial queue the block should be unqueued on. If you pass `NULL`, the main queue is used. Passing a concurrent queue results in undefined behavior.

`block`  

The block to be invoked when any of the specified times is crossed during normal rendering.

## Return Value

An object that conforms to NSObject. You must retain this value as long as you want the time observer to be invoked by the synchronizer. Pass this object to removeTimeObserver(_:) to cancel time observation.

## Discussion

Always pair a call to this method with a call to removeTimeObserver(_:). Releasing the observer without calling `removeTimeObserver(_:)` results in undefined behavior.

## See Also

### Observing Time

func addPeriodicTimeObserver(forInterval: CMTime, queue: dispatch_queue_t?, using: (CMTime) -> Void) -> Any

Requests invocation of a block during rendering at specified time intervals.

func removeTimeObserver(Any)

Cancels the specified time observer.

