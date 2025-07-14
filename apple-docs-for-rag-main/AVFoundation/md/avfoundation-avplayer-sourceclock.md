

- AVFoundation
- AVPlayer
-  sourceClock 

Instance Property

# sourceClock

A clock the player uses for item time bases.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
var sourceClock: CMClock? { get set }
```

## Discussion

The default value is `nil`. Setting an explicit source clock is useful to synchronize video-only movies with audio that plays through a different audio device.

Important

Specifying a source clock for a device other than the one playing audio may cause audio to drift out of sync.

## See Also

### Synchronizing Multiple Players

func setRate(Float, time: CMTime, atHostTime: CMTime)

Synchronizes the playback rate and time of the current item with an external source.

func preroll(atRate: Float, completionHandler: ((Bool) -> Void)?)

Begins loading media data to prime the media pipelines for playback.

func cancelPendingPrerolls()

Cancels any pending preroll requests and invokes the corresponding completion handlers, if present.

var masterClock: CMClock?

The host clock for item time bases.

Deprecated

