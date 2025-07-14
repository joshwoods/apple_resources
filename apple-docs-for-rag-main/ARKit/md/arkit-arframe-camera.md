

- ARKit
- ARFrame
-  camera 

Instance Property

# camera

Information about the camera position, orientation, and imaging parameters used to capture the frame.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
@NSCopying
var camera: ARCamera { get }
```

## See Also

### Accessing camera data

var capturedImage: CVPixelBuffer

A pixel buffer containing the image captured by the camera.

var timestamp: TimeInterval

The time at which the frame was captured.

var cameraGrainIntensity: Float

A value that specifies the amount of grain present in the camera grain texture.

var cameraGrainTexture: (any MTLTexture)?

A tileable Metal texture created by ARKit to match the visual characteristics of the current video stream.

var exifData: [String : Any]

Auxiliary data for the captured image.

