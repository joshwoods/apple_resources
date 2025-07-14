

- AVFoundation
- AVMutableVideoCompositionLayerInstruction
-  setTransform(\_:at:) 

Instance Method

# setTransform(\_:at:)

Sets the transform value at a time within the time range of the instruction.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func setTransform(
    _ transform: CGAffineTransform,
    at time: CMTime
)
```

## Parameters 

`transform`  

The transform to be applied at `time`.

`time`  

A time value within the time range of the composition instruction.

## Discussion

Sets a fixed transform to apply from the specified time until the next time at which a transform is set. This is the same as setting a flat ramp for that time range. Before the first specified time for which a transform is set, the affine transform is held constant at the value of CGAffineTransformIdentity; after the last time for which a transform is set, the affine transform is held constant at that last value.

## See Also

### Managing Properties

func setOpacity(Float, at: CMTime)

Sets the opacity value at a specific time within the time range of the instruction.

func setOpacityRamp(fromStartOpacity: Float, toEndOpacity: Float, timeRange: CMTimeRange)

Sets an opacity ramp to apply during a specified time range.

func setTransformRamp(fromStart: CGAffineTransform, toEnd: CGAffineTransform, timeRange: CMTimeRange)

Sets a transform ramp to apply during a given time range.

