

- AVFoundation
- AVSampleBufferRenderSynchronizer
-  delaysRateChangeUntilHasSufficientMediaData 

Instance Property

# delaysRateChangeUntilHasSufficientMediaData

A Boolean value that Indicates whether the playback should start immediately on rate change requests.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.4+

``` source
var delaysRateChangeUntilHasSufficientMediaData: Bool { get set }
```

## See Also

### Accessing Time Information

func currentTime() -> CMTime

Returns the current time of the synchronizer.

var timebase: CMTimebase

The synchronizer’s rendering timebase which determines how it interprets timestamps.

var rate: Float

The current playback rate.

func setRate(Float, time: CMTime)

Sets the renderer’s time and rate.

func setRate(Float, time: CMTime, atHostTime: CMTime)

Sets the playback rate and the relationship between the current time and host time.

class let rateDidChangeNotification: NSNotification.Name

The synchronizer’s rendering rate changed.

