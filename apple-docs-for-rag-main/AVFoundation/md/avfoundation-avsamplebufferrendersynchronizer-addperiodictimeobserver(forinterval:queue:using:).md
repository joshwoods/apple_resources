

- AVFoundation
- AVSampleBufferRenderSynchronizer
-  addPeriodicTimeObserver(forInterval:queue:using:) 

Instance Method

# addPeriodicTimeObserver(forInterval:queue:using:)

Requests invocation of a block during rendering at specified time intervals.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func addPeriodicTimeObserver(
    forInterval interval: CMTime,
    queue: dispatch_queue_t?,
    using block: @escaping (CMTime) -> Void
) -> Any
```

## Parameters 

`interval`  

The specified time interval requesting block invocation during rendering.

`queue`  

The serial queue the block should be unqueued on. If you pass `NULL`, the main queue is used. Passing a concurrent queue results in undefined behavior.

`block`  

The block to be invoked periodically.

## Return Value

An object that conforms to NSObject. You must retain this value as long as you want the time observer to be invoked by the synchronizer. Pass this object to removeTimeObserver(_:) to cancel time observation.

## Discussion

The block associated with this method is invoked at the specified time intervals, interpreted according to the timeline of the timebase. The block is also invoked whenever there is a time jump or rendering starts or stops.

If a very short time interval is used, the synchronizer may invoke the block less frequently than requested. However, the synchronizer will invoke the block often enough for the client to update indications of the current time appropriately in its end-user interface.

Always pair a call to this method with a call to removeTimeObserver(_:). Releasing the observer without calling `removeTimeObserver(_:)` results in undefined behavior.

## See Also

### Observing Time

func addBoundaryTimeObserver(forTimes: [NSValue], queue: dispatch_queue_t?, using: () -> Void) -> Any

Requests invocation of a block when specified times are traversed during normal rendering.

func removeTimeObserver(Any)

Cancels the specified time observer.

