

- AVFoundation
- AVVideoCompositionLayerInstruction
-  getTransformRamp(for:start:end:timeRange:) 

Instance Method

# getTransformRamp(for:start:end:timeRange:)

Obtains the transform ramp that includes a specified time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func getTransformRamp(
    for time: CMTime,
    start startTransform: UnsafeMutablePointer?,
    end endTransform: UnsafeMutablePointer?,
    timeRange: UnsafeMutablePointer?
) -> Bool
```

## Parameters 

`time`  

If a ramp with a time range that contains the specified time has been set, information about the effective ramp for that time is supplied. Otherwise, information about the first ramp that starts after the specified time is supplied.

`startTransform`  

A pointer to a float to receive the starting transform value for the transform ramp.

This value may be `NULL`.

`endTransform`  

A pointer to a float to receive the ending transform value for the transform ramp.

This value may be `NULL`.

`timeRange`  

A pointer to a `CMTimeRange` to receive the time range of the transform ramp.

This value may be `NULL`.

## Return Value

true if values are returned successfully, otherwise false. false is returned if `time` is beyond the duration of the last transform ramp that has been set.

## See Also

### Getting Opacity, Transform, and Cropping Ramps

func getOpacityRamp(for: CMTime, startOpacity: UnsafeMutablePointer&lt;Float>?, endOpacity: UnsafeMutablePointer&lt;Float>?, timeRange: UnsafeMutablePointer&lt;CMTimeRange>?) -> Bool

Obtains the opacity ramp that includes a specified time.

func getCropRectangleRamp(for: CMTime, startCropRectangle: UnsafeMutablePointer&lt;CGRect>?, endCropRectangle: UnsafeMutablePointer&lt;CGRect>?, timeRange: UnsafeMutablePointer&lt;CMTimeRange>?) -> Bool

Obtains the crop rectangle ramp that includes the specified time.

