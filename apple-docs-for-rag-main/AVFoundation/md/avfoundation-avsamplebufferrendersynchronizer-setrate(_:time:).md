

- AVFoundation
- AVSampleBufferRenderSynchronizer
-  setRate(\_:time:) 

Instance Method

# setRate(\_:time:)

Sets the renderer’s time and rate.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func setRate(
    _ rate: Float,
    time: CMTime
)
```

## Parameters 

`rate`  

The new timebase rate. This value must be greater than or equal to `0.0`.

`time`  

The new timebase time. This value must be greater than or equal to zero, or invalid.

## Discussion

This method first sets the new time and then the new rendering rate. A `rate` value of `0.0` means that playback has stopped while a `rate` value of `1.0` indicates playback should be at the natural rate of the media.

## See Also

### Accessing Time Information

func currentTime() -> CMTime

Returns the current time of the synchronizer.

var timebase: CMTimebase

The synchronizer’s rendering timebase which determines how it interprets timestamps.

var rate: Float

The current playback rate.

func setRate(Float, time: CMTime, atHostTime: CMTime)

Sets the playback rate and the relationship between the current time and host time.

class let rateDidChangeNotification: NSNotification.Name

The synchronizer’s rendering rate changed.

var delaysRateChangeUntilHasSufficientMediaData: Bool

A Boolean value that Indicates whether the playback should start immediately on rate change requests.

