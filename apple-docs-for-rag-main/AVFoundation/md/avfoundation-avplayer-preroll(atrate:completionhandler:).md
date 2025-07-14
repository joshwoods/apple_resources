

- AVFoundation
- AVPlayer
-  preroll(atRate:completionHandler:) 

Instance Method

# preroll(atRate:completionHandler:)

Begins loading media data to prime the media pipelines for playback.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
func preroll(
    atRate rate: Float,
    completionHandler: ((Bool) -> Void)? = nil
)
```

``` source
nonisolated
func preroll(atRate rate: Float) async -> Bool
```

## Parameters 

`rate`  

The playback rate to use when determining how much data to load.

`completionHandler`  

A block to execute when the player finishes the load attempt. This block takes a single Boolean parameter that contains true if the data was loaded or false if there was a problem. For example, the value might be false if the preroll was interrupted by a time change or incompatible rate change.

## Discussion

This method loads data starting at the item’s current playback time. The current rate for the playback item should always be 0 prior to calling this method. After the method calls the completion handler, you can change the item’s playback rate to begin playback.

If the player object is not ready to play (its status property is not AVPlayer.Status.readyToPlay), this method throws an exception.

## See Also

### Synchronizing Multiple Players

func setRate(Float, time: CMTime, atHostTime: CMTime)

Synchronizes the playback rate and time of the current item with an external source.

func cancelPendingPrerolls()

Cancels any pending preroll requests and invokes the corresponding completion handlers, if present.

var sourceClock: CMClock?

A clock the player uses for item time bases.

var masterClock: CMClock?

The host clock for item time bases.

Deprecated

