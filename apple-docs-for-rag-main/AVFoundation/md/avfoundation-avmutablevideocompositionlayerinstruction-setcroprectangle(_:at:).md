

- AVFoundation
- AVMutableVideoCompositionLayerInstruction
-  setCropRectangle(\_:at:) 

Instance Method

# setCropRectangle(\_:at:)

Sets the crop rectangle value at a time within the time range of the instruction.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func setCropRectangle(
    _ cropRectangle: CGRect,
    at time: CMTime
)
```

## Parameters 

`cropRectangle`  

The crop rectangle to be applied at the specified time.

`time`  

A time value within the timeRange of the composition instruction.

## Discussion

The origin of the crop rectangle is the top-left corner of the buffer clean aperture rectangle. The crop rectangle is defined in square pixel space, that is, without taking the pixel aspect ratio into account. Crop rectangles extending outside of the clean aperture, are cropped to the clean aperture.

Sets a fixed crop rectangle to apply from `time` until the next time at which a crop rectangle is set; this is the same as setting a flat ramp for that time range.

Before the first specified time for which a crop rectangle is set, the crop rectangle is held constant to CGRectInfinite and after the last time for which a crop rectangle is set, the crop rectangle is held constant at that last value.

## See Also

### Setting Crop Rectangle Values

func setCropRectangleRamp(fromStartCropRectangle: CGRect, toEndCropRectangle: CGRect, timeRange: CMTimeRange)

Sets a crop rectangle ramp to apply during the specified time range.

