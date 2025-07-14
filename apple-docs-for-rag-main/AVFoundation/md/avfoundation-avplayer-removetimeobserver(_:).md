

- AVFoundation
- AVPlayer
-  removeTimeObserver(\_:) 

Instance Method

# removeTimeObserver(\_:)

Cancels a previously registered periodic or boundary time observer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
func removeTimeObserver(_ observer: Any)
```

## Parameters 

`observer`  

An object returned by a previous call to addPeriodicTimeObserver(forInterval:queue:using:) or addBoundaryTimeObserver(forTimes:queue:using:).

## Mentioned in 

Monitoring playback progress in your app

## Discussion

Upon return, the caller is guaranteed that no new time observer blocks will begin executing. Depending on the calling thread and the queue used to add the time observer, an in-flight block may continue to execute after this method returns. You can guarantee synchronous time observer removal by enqueuing the call to `removeTimeObserver` on that queue. Alternatively, call `dispatch_sync(queue, ^{})` after `removeTimeObserver` to wait for any in-flight blocks to finish executing.

You should use this method to explicitly cancel each time observer added using addPeriodicTimeObserver(forInterval:queue:using:) and addBoundaryTimeObserver(forTimes:queue:using:).

The following shows a common implementation to remove a registered time observer:

- Swift
- Objective-C

```
func removePeriodicTimeObserver() {
    // If a time observer exists, remove it
    if let token = timeObserverToken {
        player.removeTimeObserver(token)
        timeObserverToken = nil
    }
}
```

```
- (void)removeBoundaryTimeObserver {
    if (self.timeObserverToken) {
        [self.player removeTimeObserver:self.timeObserverToken];
        self.timeObserverToken = nil;
    }
}
```

## See Also

### Observing Playback Time

func currentTime() -> CMTime

Returns the current time of the current player item.

func addPeriodicTimeObserver(forInterval: CMTime, queue: dispatch_queue_t?, using: (CMTime) -> Void) -> Any

Requests the periodic invocation of a given block during playback to report changing time.

func addBoundaryTimeObserver(forTimes: [NSValue], queue: dispatch_queue_t?, using: () -> Void) -> Any

Requests the invocation of a block when specified times are traversed during normal playback.

