

- ARKit
- ARFrame
-  cameraGrainTexture 

Instance Property

# cameraGrainTexture

A tileable Metal texture created by ARKit to match the visual characteristics of the current video stream.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var cameraGrainTexture: (any MTLTexture)? { get }
```

## Discussion

Camera grain enhances the visual cohesion of the real and augmented aspects of your user experience by enabling your app’s virtual content to take on similar image noise characteristics that naturally occur in the camera feed.

If ARSCNView is your renderer, SceneKit applies camera grain to your app’s virtual content by default. For more information, see rendersCameraGrain.

### Enable Image Noise on a Custom Renderer

For apps that display an AR experience using a custom Metal renderer, ARKit provides you with an cameraGrainTexture that matches the noise it detects in the current video stream. Set the noise texture onto your renderer to apply its characteristics to your virtual content.

The depth dimension of the image noise texture contains variations that you select at runtime based on the cameraGrainIntensity of the current frame.

## See Also

### Accessing camera data

var camera: ARCamera

Information about the camera position, orientation, and imaging parameters used to capture the frame.

var capturedImage: CVPixelBuffer

A pixel buffer containing the image captured by the camera.

var timestamp: TimeInterval

The time at which the frame was captured.

var cameraGrainIntensity: Float

A value that specifies the amount of grain present in the camera grain texture.

var exifData: [String : Any]

Auxiliary data for the captured image.

