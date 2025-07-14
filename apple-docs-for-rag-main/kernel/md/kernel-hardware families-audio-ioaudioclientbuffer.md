

- Kernel
- Hardware Families
- Audio
-  IOAudioClientBuffer 

Structure

# IOAudioClientBuffer

macOS 10.1+

``` source
typedef struct IOAudioClientBuffer {
    ...
} IOAudioClientBuffer;
```

## Topics

### Instance Properties

audioStream

bufferDataDescriptor

mNextBuffer32

mixedPosition

nextClient

nextClip

numChannels

numSampleFrames

previousClip

sourceBuffer

sourceBufferDescriptor

sourceBufferMap

unmappedSourceBuffer

userClient

## See Also

### Audio Data

IOAudioEngineNotifications

IOAudioEngineTraps

IOAudioSampleRate

IOAudioStreamFormat

IOAudioStreamFormatExtension

IOAudioTimeStamp

IOAudioClientBuffer64

IOAudioClientBufferExtendedInfo

IOAudioClientBufferExtendedInfo64

IOAudioEnginePosition

Represents a position in an audio audio engine.

IOAF_bcopy_WriteCombine

An efficient bcopy from "write combine" memory to regular memory. It is safe to assume that all memory has been copied when the function has completed

UInt64mult

