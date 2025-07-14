

- Create ML Components
- VideoReader
- VideoReader.CameraConfiguration
-  resolution 

Instance Property

# resolution

The camera resolution specifying the quality of the video output. The default values is `.high`

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var resolution: VideoReader.CameraConfiguration.Resolution
```

## See Also

### Getting the properties

var cameraPosition: VideoReader.CameraConfiguration.Position

The camera position. For an iOS device this can be either `.front` or `.rear`. For devices with just one camera this value is ignored. The default value is `.front`.

Deprecated

var frameRate: Double

The camera frame rate. The default value is 30.0 frames per second.

var pixelFormat: VideoReader.CameraConfiguration.PixelFormat

The camera pixel format. The default is `.bgra32`.

var position: VideoReader.CameraConfiguration.Position

The camera position. For an iOS device this can be either `.front` or `.rear`. For devices with just one camera this value is ignored. The default value is `.front`.

