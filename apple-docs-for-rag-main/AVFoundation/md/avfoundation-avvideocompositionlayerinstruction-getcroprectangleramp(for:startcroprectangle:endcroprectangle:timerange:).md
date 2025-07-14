

- AVFoundation
- AVVideoCompositionLayerInstruction
-  getCropRectangleRamp(for:startCropRectangle:endCropRectangle:timeRange:) 

Instance Method

# getCropRectangleRamp(for:startCropRectangle:endCropRectangle:timeRange:)

Obtains the crop rectangle ramp that includes the specified time.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func getCropRectangleRamp(
    for time: CMTime,
    startCropRectangle: UnsafeMutablePointer?,
    endCropRectangle: UnsafeMutablePointer?,
    timeRange: UnsafeMutablePointer?
) -> Bool
```

## Parameters 

`time`  

If a ramp with a time range that contains the specified time has been set, information about the effective ramp for that time is supplied. Otherwise, information about the first ramp that starts after the specified time is supplied.

`startCropRectangle`  

A pointer to a `CGRect` to receive the starting crop rectangle value for the crop rectangle ramp.

May be NULL.

`endCropRectangle`  

A pointer to a `CGRect` to receive the ending crop rectangle value for the crop rectangle ramp.

This value may be `NULL`.

`timeRange`  

A pointer to a `CMTimeRange` to receive the time range of the crop rectangle ramp.

This value may be `NULL`.

## Return Value

false will be returned if the specified time is beyond the duration of the last crop rectangle ramp that has been set.

## See Also

### Getting Opacity, Transform, and Cropping Ramps

func getOpacityRamp(for: CMTime, startOpacity: UnsafeMutablePointer&lt;Float>?, endOpacity: UnsafeMutablePointer&lt;Float>?, timeRange: UnsafeMutablePointer&lt;CMTimeRange>?) -> Bool

Obtains the opacity ramp that includes a specified time.

func getTransformRamp(for: CMTime, start: UnsafeMutablePointer&lt;CGAffineTransform>?, end: UnsafeMutablePointer&lt;CGAffineTransform>?, timeRange: UnsafeMutablePointer&lt;CMTimeRange>?) -> Bool

Obtains the transform ramp that includes a specified time.

