

- Create ML Components
- VideoReader
-  VideoReader.CameraConfiguration 

Structure

# VideoReader.CameraConfiguration

The configuration of the camera to pass to the `readCamera` method.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
struct CameraConfiguration
```

## Topics

### Creating a camera configuration

init()

Creates a camera configuration.

init(position: VideoReader.CameraConfiguration.Position, pixelFormat: VideoReader.CameraConfiguration.PixelFormat, resolution: VideoReader.CameraConfiguration.Resolution, frameRate: Double)

Creates a camera configuration.

enum PixelFormat

The camera pixel format.

enum Position

The position of the camera for an iOS device.

enum Resolution

The camera resolution.

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

var resolution: VideoReader.CameraConfiguration.Resolution

The camera resolution specifying the quality of the video output. The default values is `.high`

## Relationships

### Conforms To

- Sendable

## See Also

### Reading

static func read&lt;S>(S) async throws -> [VideoReader.AsyncFrames]

Reads a sequence of files as an array of async sequences of video frames.

static func read&lt;S, Annotation>(S) async throws -> [AnnotatedFeature&lt;VideoReader.AsyncFrames, Annotation>]

Reads a sequence of annotated files as an array of annotated async sequences of video frames.

static func readCamera(configuration: VideoReader.CameraConfiguration) async throws -> VideoReader.CameraAsyncBuffers

Reads an async sequence of video frames captured with a video camera.

static func read(contentsOf: URL) async throws -> VideoReader.AsyncFrames

Reads a video file as an async sequence of video frames.

struct AsyncFrames

An async sequence of video frames.

struct CameraAsyncBuffers

An async sequence of video frames.

