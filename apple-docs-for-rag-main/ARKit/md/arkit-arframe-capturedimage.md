

- ARKit
- ARFrame
-  capturedImage 

Instance Property

# capturedImage

A pixel buffer containing the image captured by the camera.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var capturedImage: CVPixelBuffer { get }
```

## Mentioned in 

Displaying an AR Experience with Metal

## Discussion

ARKit captures pixel buffers in a full-range planar YCbCr format (also known as YUV) format according to the ITU R. 601-4 standard. (You can verify this by checking the kCVImageBufferYCbCrMatrixKey pixel buffer attachment.)

Unlike some uses of that standard, ARKit captures full-range color space values, not video-range values. To correctly render these images on a device display, you’ll need to access the luma and chroma planes of the pixel buffer and convert full-range YCbCr values to an sRGB (or ITU R. 709) format according to the ITU-T T.871 specification.

The following matrix (shown in Metal shader syntax) performs this conversion when multiplied by a 4-element vector (containing Y’, Cb, Cr values and an “alpha” value of 1.0):

```
```

For more details, see Displaying an AR Experience with Metal, or use the Metal variant of the AR app template when creating a new project in Xcode.

## See Also

### Accessing camera data

var camera: ARCamera

Information about the camera position, orientation, and imaging parameters used to capture the frame.

var timestamp: TimeInterval

The time at which the frame was captured.

var cameraGrainIntensity: Float

A value that specifies the amount of grain present in the camera grain texture.

var cameraGrainTexture: (any MTLTexture)?

A tileable Metal texture created by ARKit to match the visual characteristics of the current video stream.

var exifData: [String : Any]

Auxiliary data for the captured image.

