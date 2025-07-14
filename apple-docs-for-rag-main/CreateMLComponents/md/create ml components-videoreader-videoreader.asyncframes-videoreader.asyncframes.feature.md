

- Create ML Components
- VideoReader
- VideoReader.AsyncFrames
-  VideoReader.AsyncFrames.Feature 

Type Alias

# VideoReader.AsyncFrames.Feature

The feature type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
typealias Feature = CIImage
```

## See Also

### Creating an iterator

func makeAsyncIterator() -> VideoReader.AsyncFrames.Iterator

Constructs an iterator.

struct Iterator

An async iterator of video frames.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

