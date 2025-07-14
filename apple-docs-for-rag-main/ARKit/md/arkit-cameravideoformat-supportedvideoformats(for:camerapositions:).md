

- ARKit
- CameraVideoFormat
-  supportedVideoFormats(for:cameraPositions:) 

Type Method

# supportedVideoFormats(for:cameraPositions:)

Returns the video formats the provided camera type and camera position supports.

visionOS 2.0+

``` source
static func supportedVideoFormats(
    for cameraType: CameraFrameProvider.CameraType,
    cameraPositions: [CameraFrameProvider.CameraPosition]
) -> [CameraVideoFormat]
```

## Parameters 

`cameraType`  

The camera type.

`cameraPositions`  

The camera position.

## Return Value

An array of camera video formats.

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

var maxFrameDuration: Float

The maximum frame duration for this video format, in seconds.

var minFrameDuration: Float

The minimum frame duration for this video format, in seconds.

var description: String

A textual representation of this camera video format.

