

- AVFoundation
- AVMutableAudioMixInputParameters
-  setVolume(\_:at:) 

Instance Method

# setVolume(\_:at:)

Sets the value of the audio volume starting at the specified time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func setVolume(
    _ volume: Float,
    at time: CMTime
)
```

## Parameters 

`volume`  

The volume. The value must be between `0.0` and `1.0`.

`time`  

The start time at which to set the volume.

## Discussion

This method adds a volume ramp starting at `time`. This volume setting remains in effect until the end of the track unless you set a different volume level to start at a later time.

## See Also

### Setting the Volume

func setVolumeRamp(fromStartVolume: Float, toEndVolume: Float, timeRange: CMTimeRange)

Sets a volume ramp to apply during a specified time range.

