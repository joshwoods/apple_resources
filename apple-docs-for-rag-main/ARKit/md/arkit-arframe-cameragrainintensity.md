

- ARKit
- ARFrame
-  cameraGrainIntensity 

Instance Property

# cameraGrainIntensity

A value that specifies the amount of grain present in the camera grain texture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var cameraGrainIntensity: Float { get }
```

## Discussion

This property is normalized within the range \[0..1\], where zero specifies no grain, and one specifies the maximum amount of grain.

When you apply this value to the depth component of the cameraGrainTexture, you select among variations of visual image noise data stored in the Metal texture that conceptually match this level of intensity.

## See Also

### Accessing camera data

var camera: ARCamera

Information about the camera position, orientation, and imaging parameters used to capture the frame.

var capturedImage: CVPixelBuffer

A pixel buffer containing the image captured by the camera.

var timestamp: TimeInterval

The time at which the frame was captured.

var cameraGrainTexture: (any MTLTexture)?

A tileable Metal texture created by ARKit to match the visual characteristics of the current video stream.

var exifData: [String : Any]

Auxiliary data for the captured image.

