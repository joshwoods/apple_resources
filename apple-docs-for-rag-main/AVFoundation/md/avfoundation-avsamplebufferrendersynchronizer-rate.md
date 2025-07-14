

- AVFoundation
- AVSampleBufferRenderSynchronizer
-  rate 

Instance Property

# rate

The current playback rate.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var rate: Float { get set }
```

## Discussion

A value of `0.0` means playback has stopped. A value of `1.0` tells the renderer to play at the natural rate of the media. This property must be greater than or equal to `0.0`.

## See Also

### Accessing Time Information

func currentTime() -> CMTime

Returns the current time of the synchronizer.

var timebase: CMTimebase

The synchronizer’s rendering timebase which determines how it interprets timestamps.

func setRate(Float, time: CMTime)

Sets the renderer’s time and rate.

func setRate(Float, time: CMTime, atHostTime: CMTime)

Sets the playback rate and the relationship between the current time and host time.

class let rateDidChangeNotification: NSNotification.Name

The synchronizer’s rendering rate changed.

var delaysRateChangeUntilHasSufficientMediaData: Bool

A Boolean value that Indicates whether the playback should start immediately on rate change requests.

