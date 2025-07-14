

- AVFoundation
- AVSampleBufferRenderSynchronizer
-  timebase 

Instance Property

# timebase

The synchronizer’s rendering timebase which determines how it interprets timestamps.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var timebase: CMTimebase { get }
```

## Discussion

The default for this property is the clock for an added AVSampleBufferAudioRenderer object. If you haven’t added a renderer, the timebase is the system host clock.

## See Also

### Accessing Time Information

func currentTime() -> CMTime

Returns the current time of the synchronizer.

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

