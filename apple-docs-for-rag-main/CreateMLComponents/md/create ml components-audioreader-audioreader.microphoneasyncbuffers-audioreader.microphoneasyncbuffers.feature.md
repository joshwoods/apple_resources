

- Create ML Components
- AudioReader
- AudioReader.MicrophoneAsyncBuffers
-  AudioReader.MicrophoneAsyncBuffers.Feature 

Type Alias

# AudioReader.MicrophoneAsyncBuffers.Feature

The feature type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
typealias Feature = AVAudioPCMBuffer
```

## See Also

### Creating an iterator

func makeAsyncIterator() -> AudioReader.MicrophoneAsyncBuffers.Iterator

Constructs an iterator.

class Iterator

An async iterator of audio frames.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

