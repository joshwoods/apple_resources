

- AVFAudio
- AVAudioPCMBuffer
-  init(pcmFormat:frameCapacity:) 

Initializer

# init(pcmFormat:frameCapacity:)

Creates a PCM audio buffer instance for PCM audio data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    pcmFormat format: AVAudioFormat,
    frameCapacity: AVAudioFrameCount
)
```

## Parameters 

`format`  

The format of the PCM audio the buffer contains.

`frameCapacity`  

The capacity of the buffer in PCM sample frames.

## Return Value

A new AVAudioPCMBuffer instance, or `nil` if it’s not possible.

## Discussion

The method returns `nil` due to the following reasons:

- The format has zero bytes per frame.

- The system can’t represent the buffer byte capacity as an unsigned bit-32 integer.

## See Also

### Related Documentation

var frameLength: AVAudioFrameCount

The current number of valid sample frames in the buffer.

var frameCapacity: AVAudioFrameCount

The buffer’s capacity, in audio sample frames.

### Creating a PCM Audio Buffer

init?(pcmFormat: AVAudioFormat, bufferListNoCopy: UnsafePointer&lt;AudioBufferList>, deallocator: ((UnsafePointer&lt;AudioBufferList>) -> Void)?)

Creates a PCM audio buffer instance without copying samples, for PCM audio data, with a specified buffer list and a deallocator closure.

