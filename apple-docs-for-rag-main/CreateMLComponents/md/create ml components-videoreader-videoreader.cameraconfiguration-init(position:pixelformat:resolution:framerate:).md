

- Create ML Components
- VideoReader
- VideoReader.CameraConfiguration
-  init(position:pixelFormat:resolution:frameRate:) 

Initializer

# init(position:pixelFormat:resolution:frameRate:)

Creates a camera configuration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
init(
    position: VideoReader.CameraConfiguration.Position = .front,
    pixelFormat: VideoReader.CameraConfiguration.PixelFormat = .bgra32,
    resolution: VideoReader.CameraConfiguration.Resolution = .high,
    frameRate: Double = 30.0
)
```

## Parameters 

`position`  

The position of the camera. The default value is `.front`. For devices with just one camera this value is ignored.

`pixelFormat`  

The pixel format of the camera frames. The default is `.bgra32`.

`resolution`  

The camera resolution. The default values is `.high`.

`frameRate`  

The camera frame rate. The default value is 30.0 frames per second.

## See Also

### Creating a camera configuration

init()

Creates a camera configuration.

enum PixelFormat

The camera pixel format.

enum Position

The position of the camera for an iOS device.

enum Resolution

The camera resolution.

