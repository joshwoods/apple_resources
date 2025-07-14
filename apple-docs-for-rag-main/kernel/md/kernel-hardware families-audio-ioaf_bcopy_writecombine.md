

- Kernel
- Hardware Families
- Audio
-  IOAF_bcopy_WriteCombine 

Function

# IOAF_bcopy_WriteCombine

An efficient bcopy from "write combine" memory to regular memory. It is safe to assume that all memory has been copied when the function has completed

macOS 10.7+

``` source
void IOAF_bcopy_WriteCombine(const void *src, void *dest, unsigned int count);
```

## Parameters 

`src`  

Pointer to the data to convert

`dest`  

Pointer to the converted data

`count`  

The number of items to convert

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

IOAudioEnginePosition

Represents a position in an audio audio engine.

UInt64mult

