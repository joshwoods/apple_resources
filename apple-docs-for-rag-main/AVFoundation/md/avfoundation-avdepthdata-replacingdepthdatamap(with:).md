

- AVFoundation
- AVDepthData
-  replacingDepthDataMap(with:) 

Instance Method

# replacingDepthDataMap(with:)

Returns a derivative depth data object by replacing the depth data map.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func replacingDepthDataMap(with pixelBuffer: CVPixelBuffer) throws -> Self
```

## Parameters 

`pixelBuffer`  

A pixel buffer containing depth or disparity information in a compatible format.

## Return Value

A new depth data object containing the pixel buffer.

## Discussion

If you apply simple transforms to media containing depth data, you can use the applyingExifOrientation(_:) method to apply parallel transforms to the corresponding depth data. More complex transforms and edits require creating a derivative depth map reflecting whatever edits you make to the corresponding image. In such cases, use this replacingDepthDataMap(with:) method to create a derivative depth data object.

Note

This method cannot ensure correspondence between an arbitrarily edited depth map and the camera parameters that generated the initial depth map, so the new depth data object’s cameraCalibrationData property is always `nil`.

## See Also

### Transforming and Processing

func applyingExifOrientation(CGImagePropertyOrientation) -> Self

Returns a derivative depth data object by mirroring or rotating it to the specified orientation.

func converting(toDepthDataType: OSType) -> Self

Returns a derivative depth data object by converting the depth data map to the specified data type.

var availableDepthDataTypes: [OSType]

The list of depth data formats to which you can convert this depth data.

