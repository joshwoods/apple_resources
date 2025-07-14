

- AVFoundation
- AVSampleBufferRenderSynchronizer
-  removeTimeObserver(\_:) 

Instance Method

# removeTimeObserver(\_:)

Cancels the specified time observer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func removeTimeObserver(_ observer: Any)
```

## Parameters 

`observer`  

The time observer to be cancelled.

## Discussion

Use this method to explicitly cancel time observers added using addPeriodicTimeObserver(forInterval:queue:using:) or addBoundaryTimeObserver(forTimes:queue:using:)

Upon return, the caller is guaranteed that no new time observer blocks will begin executing. Depending on the calling thread and the queue used to add the time observer, an in-flight block may continue to execute after this method returns. You can guarantee synchronous time observer removal by enqueuing the call to `removeTimeObserver:` on that queue. Call sync(execute:) after `removeTimeObserver:` to wait for any in-flight blocks to finish executing.

## See Also

### Observing Time

func addPeriodicTimeObserver(forInterval: CMTime, queue: dispatch_queue_t?, using: (CMTime) -> Void) -> Any

Requests invocation of a block during rendering at specified time intervals.

func addBoundaryTimeObserver(forTimes: [NSValue], queue: dispatch_queue_t?, using: () -> Void) -> Any

Requests invocation of a block when specified times are traversed during normal rendering.

