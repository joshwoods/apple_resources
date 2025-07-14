

- Create ML Components
- VideoReader
-  read(contentsOf:) 

Type Method

# read(contentsOf:)

Reads a video file as an async sequence of video frames.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
static func read(contentsOf url: URL) async throws -> VideoReader.AsyncFrames
```

## Parameters 

`url`  

A video file URL.

## Return Value

An async sequence of `VideoFrames`.

## See Also

### Reading

static func read&lt;S>(S) async throws -> [VideoReader.AsyncFrames]

Reads a sequence of files as an array of async sequences of video frames.

static func read&lt;S, Annotation>(S) async throws -> [AnnotatedFeature&lt;VideoReader.AsyncFrames, Annotation>]

Reads a sequence of annotated files as an array of annotated async sequences of video frames.

static func readCamera(configuration: VideoReader.CameraConfiguration) async throws -> VideoReader.CameraAsyncBuffers

Reads an async sequence of video frames captured with a video camera.

struct AsyncFrames

An async sequence of video frames.

struct CameraAsyncBuffers

An async sequence of video frames.

struct CameraConfiguration

The configuration of the camera to pass to the `readCamera` method.

