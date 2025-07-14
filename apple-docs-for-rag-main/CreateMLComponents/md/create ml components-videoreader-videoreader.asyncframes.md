

- Create ML Components
- VideoReader
-  VideoReader.AsyncFrames 

Structure

# VideoReader.AsyncFrames

An async sequence of video frames.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct AsyncFrames
```

## Overview

This sequence allows iterating through the file only once.

## Topics

### Getting the properties

var count: Int?

The number of frames. For this sequence count is always nil.

let frameSize: CGSize

The frame size.

let nominalFrameRate: Float

The nominal frame rate.

let timescale: CMTimeScale

The timescale of the video track.

let url: URL

The video file URL, used when throwing an error.

let videoDuration: CMTime

The video duration.

### Creating an iterator

func makeAsyncIterator() -> VideoReader.AsyncFrames.Iterator

Constructs an iterator.

struct Iterator

An async iterator of video frames.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Feature

The feature type.

### Type Aliases

typealias Element

The type of element produced by this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence
- TemporalSequence

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

struct CameraAsyncBuffers

An async sequence of video frames.

struct CameraConfiguration

The configuration of the camera to pass to the `readCamera` method.

