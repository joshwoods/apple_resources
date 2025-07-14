

- AVFoundation
- AVMutableAudioMixInputParameters
-  setVolumeRamp(fromStartVolume:toEndVolume:timeRange:) 

Instance Method

# setVolumeRamp(fromStartVolume:toEndVolume:timeRange:)

Sets a volume ramp to apply during a specified time range.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func setVolumeRamp(
    fromStartVolume startVolume: Float,
    toEndVolume endVolume: Float,
    timeRange: CMTimeRange
)
```

## Parameters 

`startVolume`  

The starting volume. The value must be between `0.0` and 1.0.

`endVolume`  

The end volume. The value must be between `0.0` and `1.0`.

`timeRange`  

The time range over which to apply the ramp.

## See Also

### Setting the Volume

func setVolume(Float, at: CMTime)

Sets the value of the audio volume starting at the specified time.

