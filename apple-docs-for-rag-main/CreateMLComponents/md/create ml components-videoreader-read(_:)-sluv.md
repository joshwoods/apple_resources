

- Create ML Components
- VideoReader
-  read(\_:) 

Type Method

# read(\_:)

Reads a sequence of annotated files as an array of annotated async sequences of video frames.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
static func read(_ annotatedFiles: S) async throws -> [AnnotatedFeature] where S : Sequence, Annotation : Equatable, Annotation : Sendable, S.Element == AnnotatedFeature
```

## Parameters 

`annotatedFiles`  

A sequence of annotated URLs.

## Return Value

An array of annotated async sequences.

## See Also

### Reading

static func read&lt;S>(S) async throws -> [VideoReader.AsyncFrames]

Reads a sequence of files as an array of async sequences of video frames.

static func readCamera(configuration: VideoReader.CameraConfiguration) async throws -> VideoReader.CameraAsyncBuffers

Reads an async sequence of video frames captured with a video camera.

static func read(contentsOf: URL) async throws -> VideoReader.AsyncFrames

Reads a video file as an async sequence of video frames.

struct AsyncFrames

An async sequence of video frames.

struct CameraAsyncBuffers

An async sequence of video frames.

struct CameraConfiguration

The configuration of the camera to pass to the `readCamera` method.

