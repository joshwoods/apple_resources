

- AVFoundation
- AVPlayer
-  currentTime() 

Instance Method

# currentTime()

Returns the current time of the current player item.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
func currentTime() -> CMTime
```

## Return Value

The current time of the current player item.

## Discussion

This property isn’t key-value observable. To observe the player’s time, use addPeriodicTimeObserver(forInterval:queue:using:) or addBoundaryTimeObserver(forTimes:queue:using:).

## See Also

### Observing Playback Time

func addPeriodicTimeObserver(forInterval: CMTime, queue: dispatch_queue_t?, using: (CMTime) -> Void) -> Any

Requests the periodic invocation of a given block during playback to report changing time.

func addBoundaryTimeObserver(forTimes: [NSValue], queue: dispatch_queue_t?, using: () -> Void) -> Any

Requests the invocation of a block when specified times are traversed during normal playback.

func removeTimeObserver(Any)

Cancels a previously registered periodic or boundary time observer.

