

- AVFoundation
- AVCameraCalibrationData
-  intrinsicMatrixReferenceDimensions 

Instance Property

# intrinsicMatrixReferenceDimensions

The image dimensions to which the camera’s intrinsic matrix values are relative.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var intrinsicMatrixReferenceDimensions: CGSize { get }
```

## Discussion

The intrinsicMatrix property measures focal length and principal point offset in pixels, but those values are meaningful only in the context of an image of this size.

## See Also

### Mapping Pixels to Scene Geometry

var intrinsicMatrix: matrix_float3x3

A matrix that relates a camera’s internal properties to an ideal pinhole-camera model.

var extrinsicMatrix: matrix_float4x3

A matrix relating a camera’s position and orientation to a world or scene coordinate system.

var pixelSize: Float

The size, in millimeters, of one image pixel.

