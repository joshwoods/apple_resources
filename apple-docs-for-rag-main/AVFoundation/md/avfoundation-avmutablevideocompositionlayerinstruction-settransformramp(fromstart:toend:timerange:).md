

- AVFoundation
- AVMutableVideoCompositionLayerInstruction
-  setTransformRamp(fromStart:toEnd:timeRange:) 

Instance Method

# setTransformRamp(fromStart:toEnd:timeRange:)

Sets a transform ramp to apply during a given time range.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func setTransformRamp(
    fromStart startTransform: CGAffineTransform,
    toEnd endTransform: CGAffineTransform,
    timeRange: CMTimeRange
)
```

## Parameters 

`startTransform`  

The transform to be applied at the starting time of `timeRange`.

`endTransform`  

The transform to be applied at the end time of `timeRange`.

`timeRange`  

The time range over which the value of the transform is interpolated between `startTransform` and `endTransform`.

## Discussion

During a transform ramp, the affine transform is interpolated between the values set at the ramp’s start time and end time. Before the first specified time for which a transform is set, the affine transform is held constant at the value of CGAffineTransformIdentity; after the last time for which a transform is set, the affine transform is held constant at that last value.

## See Also

### Managing Properties

func setOpacity(Float, at: CMTime)

Sets the opacity value at a specific time within the time range of the instruction.

func setOpacityRamp(fromStartOpacity: Float, toEndOpacity: Float, timeRange: CMTimeRange)

Sets an opacity ramp to apply during a specified time range.

func setTransform(CGAffineTransform, at: CMTime)

Sets the transform value at a time within the time range of the instruction.

