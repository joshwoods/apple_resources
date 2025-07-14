

- AVFoundation
- AVSampleBufferRenderSynchronizer
-  currentTime() 

Instance Method

# currentTime()

Returns the current time of the synchronizer.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func currentTime() -> CMTime
```

## Return Value

A CMTime object.

## See Also

### Accessing Time Information

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

var delaysRateChangeUntilHasSufficientMediaData: Bool

A Boolean value that Indicates whether the playback should start immediately on rate change requests.

