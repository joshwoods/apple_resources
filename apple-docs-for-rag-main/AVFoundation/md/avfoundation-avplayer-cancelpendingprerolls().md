

- AVFoundation
- AVPlayer
-  cancelPendingPrerolls() 

Instance Method

# cancelPendingPrerolls()

Cancels any pending preroll requests and invokes the corresponding completion handlers, if present.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
func cancelPendingPrerolls()
```

## Discussion

This method cancels and releases the completion handlers for any pending prerolls. The finished parameter of the completion handlers passed to preroll(atRate:completionHandler:) will be set to `false`.

## See Also

### Synchronizing Multiple Players

func setRate(Float, time: CMTime, atHostTime: CMTime)

Synchronizes the playback rate and time of the current item with an external source.

func preroll(atRate: Float, completionHandler: ((Bool) -> Void)?)

Begins loading media data to prime the media pipelines for playback.

var sourceClock: CMClock?

A clock the player uses for item time bases.

var masterClock: CMClock?

The host clock for item time bases.

Deprecated

