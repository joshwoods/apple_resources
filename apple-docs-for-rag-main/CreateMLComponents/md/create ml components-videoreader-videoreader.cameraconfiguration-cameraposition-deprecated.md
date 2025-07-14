

- Create ML Components
- VideoReader
- VideoReader.CameraConfiguration
-  cameraPosition Deprecated

Instance Property

# cameraPosition

The camera position. For an iOS device this can be either `.front` or `.rear`. For devices with just one camera this value is ignored. The default value is `.front`.

iOS 16.0–17.0DeprecatediPadOS 16.0–17.0DeprecatedMac Catalyst 16.0–17.0DeprecatedmacOS 13.0–14.0DeprecatedvisionOS 1.0+

``` source
var cameraPosition: VideoReader.CameraConfiguration.Position { get }
```

Deprecated

Use the position property instead.

## See Also

### Getting the properties

var frameRate: Double

The camera frame rate. The default value is 30.0 frames per second.

var pixelFormat: VideoReader.CameraConfiguration.PixelFormat

The camera pixel format. The default is `.bgra32`.

var position: VideoReader.CameraConfiguration.Position

The camera position. For an iOS device this can be either `.front` or `.rear`. For devices with just one camera this value is ignored. The default value is `.front`.

var resolution: VideoReader.CameraConfiguration.Resolution

The camera resolution specifying the quality of the video output. The default values is `.high`

