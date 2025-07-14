

- Create ML Components
- VideoReader
- VideoReader.CameraAsyncBuffers
-  VideoReader.CameraAsyncBuffers.Feature 

Type Alias

# VideoReader.CameraAsyncBuffers.Feature

The feature type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
typealias Feature = CIImage
```

## See Also

### Creating an iterator

func makeAsyncIterator() -> VideoReader.CameraAsyncBuffers.Iterator

Constructs an iterator.

class Iterator

An async iterator of video frames.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

