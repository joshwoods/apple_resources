

- Kernel
- Hardware Families
- Audio
-  IOAudioEnginePosition 

Structure

# IOAudioEnginePosition

Represents a position in an audio audio engine.

macOS 10.1+

``` source
typedef struct IOAudioEnginePosition {
    ...
} IOAudioEnginePosition;
```

## Overview

This position is based on the sample frame within a loop around the sample buffer, and the loop count which starts at 0 when the audio engine begins playback.

## Topics

### Instance Properties

fLoopCount

fSampleFrame

## See Also

### Audio Data

IOAudioEngineNotifications

IOAudioEngineTraps

IOAudioSampleRate

IOAudioStreamFormat

IOAudioStreamFormatExtension

IOAudioTimeStamp

IOAudioClientBuffer

IOAudioClientBuffer64

IOAudioClientBufferExtendedInfo

IOAudioClientBufferExtendedInfo64

IOAF_bcopy_WriteCombine

An efficient bcopy from "write combine" memory to regular memory. It is safe to assume that all memory has been copied when the function has completed

UInt64mult

