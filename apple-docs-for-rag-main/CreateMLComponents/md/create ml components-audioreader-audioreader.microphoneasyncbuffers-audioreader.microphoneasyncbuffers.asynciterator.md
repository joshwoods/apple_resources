

- Create ML Components
- AudioReader
- AudioReader.MicrophoneAsyncBuffers
-  AudioReader.MicrophoneAsyncBuffers.AsyncIterator 

Type Alias

# AudioReader.MicrophoneAsyncBuffers.AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
typealias AsyncIterator = AudioReader.MicrophoneAsyncBuffers.Iterator
```

## See Also

### Creating an iterator

func makeAsyncIterator() -> AudioReader.MicrophoneAsyncBuffers.Iterator

Constructs an iterator.

class Iterator

An async iterator of audio frames.

typealias Feature

The feature type.

