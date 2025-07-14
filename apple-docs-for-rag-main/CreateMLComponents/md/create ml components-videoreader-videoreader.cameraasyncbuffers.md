

- Create ML Components
- VideoReader
-  VideoReader.CameraAsyncBuffers 

Structure

# VideoReader.CameraAsyncBuffers

An async sequence of video frames.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
struct CameraAsyncBuffers
```

## Overview

This sequence allows iterating through the camera frames. Only one iterator can be created per sequence.

## Topics

### Getting the capture session

var captureSession: AVCaptureSession

The capture session.

### Creating an iterator

func makeAsyncIterator() -> VideoReader.CameraAsyncBuffers.Iterator

Constructs an iterator.

class Iterator

An async iterator of video frames.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Feature

The feature type.

### Instance Properties

var count: Int?

The number of frames. For this sequence count is always nil.

### Type Aliases

typealias Element

The type of element produced by this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence
- Sendable
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

struct AsyncFrames

An async sequence of video frames.

struct CameraConfiguration

The configuration of the camera to pass to the `readCamera` method.

