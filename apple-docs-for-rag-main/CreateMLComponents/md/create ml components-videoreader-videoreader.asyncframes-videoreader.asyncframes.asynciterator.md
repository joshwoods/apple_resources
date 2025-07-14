

- Create ML Components
- VideoReader
- VideoReader.AsyncFrames
-  VideoReader.AsyncFrames.AsyncIterator 

Type Alias

# VideoReader.AsyncFrames.AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
typealias AsyncIterator = VideoReader.AsyncFrames.Iterator
```

## See Also

### Creating an iterator

func makeAsyncIterator() -> VideoReader.AsyncFrames.Iterator

Constructs an iterator.

struct Iterator

An async iterator of video frames.

typealias Feature

The feature type.

