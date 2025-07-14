

- Create ML Components
- VideoReader
-  readCamera(configuration:) 

Type Method

# readCamera(configuration:)

Reads an async sequence of video frames captured with a video camera.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
static func readCamera(configuration: VideoReader.CameraConfiguration) async throws -> VideoReader.CameraAsyncBuffers
```

## Parameters 

`configuration`  

The camera configuration

## Return Value

An async sequence of camera video frames.

## See Also

### Reading

static func read&lt;S>(S) async throws -> [VideoReader.AsyncFrames]

Reads a sequence of files as an array of async sequences of video frames.

static func read&lt;S, Annotation>(S) async throws -> [AnnotatedFeature&lt;VideoReader.AsyncFrames, Annotation>]

Reads a sequence of annotated files as an array of annotated async sequences of video frames.

static func read(contentsOf: URL) async throws -> VideoReader.AsyncFrames

Reads a video file as an async sequence of video frames.

struct AsyncFrames

An async sequence of video frames.

struct CameraAsyncBuffers

An async sequence of video frames.

struct CameraConfiguration

The configuration of the camera to pass to the `readCamera` method.

