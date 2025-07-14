

- AVFoundation
- AVVideoCompositionLayerInstruction
-  getOpacityRamp(for:startOpacity:endOpacity:timeRange:) 

Instance Method

# getOpacityRamp(for:startOpacity:endOpacity:timeRange:)

Obtains the opacity ramp that includes a specified time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func getOpacityRamp(
    for time: CMTime,
    startOpacity: UnsafeMutablePointer?,
    endOpacity: UnsafeMutablePointer?,
    timeRange: UnsafeMutablePointer?
) -> Bool
```

## Parameters 

`time`  

If a ramp with a time range that contains the specified time has been set, information about the effective ramp for that time is supplied. Otherwise, information about the first ramp that starts after the specified time is supplied.

`startOpacity`  

A pointer to a float to receive the starting opacity value for the opacity ramp.

This value may be `NULL`.

`endOpacity`  

A pointer to a float to receive the ending opacity value for the opacity ramp.

This value may be `NULL`.

`timeRange`  

A pointer to a `CMTimeRange` to receive the time range of the opacity ramp.

This value may be `NULL`.

## Return Value

true if values are returned successfully, otherwise false. false is returned if `time` is beyond the duration of the last opacity ramp that has been set.

## See Also

### Getting Opacity, Transform, and Cropping Ramps

func getTransformRamp(for: CMTime, start: UnsafeMutablePointer&lt;CGAffineTransform>?, end: UnsafeMutablePointer&lt;CGAffineTransform>?, timeRange: UnsafeMutablePointer&lt;CMTimeRange>?) -> Bool

Obtains the transform ramp that includes a specified time.

func getCropRectangleRamp(for: CMTime, startCropRectangle: UnsafeMutablePointer&lt;CGRect>?, endCropRectangle: UnsafeMutablePointer&lt;CGRect>?, timeRange: UnsafeMutablePointer&lt;CMTimeRange>?) -> Bool

Obtains the crop rectangle ramp that includes the specified time.

