

- AVFoundation
- AVPlayer
-  masterClock Deprecated

Instance Property

# masterClock

The host clock for item time bases.

iOS 6.0–18.0DeprecatediPadOS 6.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.8–15.0DeprecatedtvOS 9.0–18.0DeprecatedwatchOS 1.0–11.0Deprecated

``` source
nonisolated
var masterClock: CMClock? { get set }
```

Deprecated

Use sourceClock instead.

## Discussion

The default value of this property is `NULL`, which means that the host clock is the automatic choice. When non-`NULL`, this property overrides the automatic choice of host clock for item time bases. This is most useful when you’re synchronizing video-only movies with audio from another source.

Important

If you specify a host clock other than the appropriate audio device’s clock, the audio may drift out of sync.

## See Also

### Synchronizing Multiple Players

func setRate(Float, time: CMTime, atHostTime: CMTime)

Synchronizes the playback rate and time of the current item with an external source.

func preroll(atRate: Float, completionHandler: ((Bool) -> Void)?)

Begins loading media data to prime the media pipelines for playback.

func cancelPendingPrerolls()

Cancels any pending preroll requests and invokes the corresponding completion handlers, if present.

var sourceClock: CMClock?

A clock the player uses for item time bases.

