

- ARKit
- CameraVideoFormat
-  maxFrameDuration 

Instance Property

# maxFrameDuration

The maximum frame duration for this video format, in seconds.

visionOS 2.0+

``` source
var maxFrameDuration: Float { get }
```

## See Also

### Getting camera video format information

var cameraPositions: [CameraFrameProvider.CameraPosition]

The camera positions for this video format.

var cameraType: CameraFrameProvider.CameraType

The camera type for this video format.

var frameSize: CGSize

The frame size for this video format.

var pixelFormat: OSType

The pixel format for this video format.

var minFrameDuration: Float

The minimum frame duration for this video format, in seconds.

static func supportedVideoFormats(for: CameraFrameProvider.CameraType, cameraPositions: [CameraFrameProvider.CameraPosition]) -> [CameraVideoFormat]

Returns the video formats the provided camera type and camera position supports.

var description: String

A textual representation of this camera video format.

