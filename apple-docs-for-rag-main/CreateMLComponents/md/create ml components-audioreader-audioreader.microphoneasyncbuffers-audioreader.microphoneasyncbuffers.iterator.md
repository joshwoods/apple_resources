

- Create ML Components
- AudioReader
- AudioReader.MicrophoneAsyncBuffers
-  AudioReader.MicrophoneAsyncBuffers.Iterator 

Class

# AudioReader.MicrophoneAsyncBuffers.Iterator

An async iterator of audio frames.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
final class Iterator
```

## Topics

### Getting the next element

func next() async throws -> TemporalFeature&lt;AudioReader.MicrophoneAsyncBuffers.Feature>?

Advances to the next element and returns it, or nil if no next element exists.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

## See Also

### Creating an iterator

func makeAsyncIterator() -> AudioReader.MicrophoneAsyncBuffers.Iterator

Constructs an iterator.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Feature

The feature type.

