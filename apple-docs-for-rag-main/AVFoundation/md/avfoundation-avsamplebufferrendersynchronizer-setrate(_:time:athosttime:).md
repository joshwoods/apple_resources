

- AVFoundation
- AVSampleBufferRenderSynchronizer
-  setRate(\_:time:atHostTime:) 

Instance Method

# setRate(\_:time:atHostTime:)

Sets the playback rate and the relationship between the current time and host time.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.4+

``` source
func setRate(
    _ rate: Float,
    time: CMTime,
    atHostTime hostTime: CMTime
)
```

## Parameters 

`rate`  

A new timebase rate. This value must be greater than or equal to `0.0`.

`time`  

A new timebase time. This value must be greater than or equal to zero, or invalid.

`hostTime`  

A new host time. This value must be greater than or equal to zero, or invalid.

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

class let rateDidChangeNotification: NSNotification.Name

The synchronizer’s rendering rate changed.

var delaysRateChangeUntilHasSufficientMediaData: Bool

A Boolean value that Indicates whether the playback should start immediately on rate change requests.

