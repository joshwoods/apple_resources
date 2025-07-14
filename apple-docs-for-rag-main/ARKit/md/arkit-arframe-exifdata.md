

- ARKit
- ARFrame
-  exifData 

Instance Property

# exifData

Auxiliary data for the captured image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var exifData: [String : Any] { get }
```

## Discussion

The system’s image capture pipeline produces pixel data and auxiliary information for each exposure. The AR frame exposes this pixel data through capturedImage and the auxilliary info through this property (exifData). Example EXIF data includes camera manufacturer, orientation, compression, resolution, exposure, and the date and time that the exposure occurred.

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

var cameraGrainTexture: (any MTLTexture)?

A tileable Metal texture created by ARKit to match the visual characteristics of the current video stream.

