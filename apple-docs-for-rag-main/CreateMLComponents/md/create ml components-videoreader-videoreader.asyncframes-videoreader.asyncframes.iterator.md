

- Create ML Components
- VideoReader
- VideoReader.AsyncFrames
-  VideoReader.AsyncFrames.Iterator 

Structure

# VideoReader.AsyncFrames.Iterator

An async iterator of video frames.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct Iterator
```

## Topics

### Getting the next element

func next() async throws -> TemporalFeature&lt;CIImage>?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

## See Also

### Creating an iterator

func makeAsyncIterator() -> VideoReader.AsyncFrames.Iterator

Constructs an iterator.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Feature

The feature type.

