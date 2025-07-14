

- Create ML Components
- AudioReader
- AudioReader.AsyncBuffers
-  AudioReader.AsyncBuffers.AsyncIterator 

Type Alias

# AudioReader.AsyncBuffers.AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
typealias AsyncIterator = AudioReader.AsyncBuffers.Iterator
```

## See Also

### Creating an iterator

func makeAsyncIterator() -> AudioReader.AsyncBuffers.Iterator

Constructs an iterator.

struct Iterator

An async iterator of audio buffers.

typealias Feature

The feature type.

