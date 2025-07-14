

- Kernel
- Hardware Families
- Audio
-  IOAudioStream 

Class

# IOAudioStream

This class wraps a single sample buffer in an audio driver.

macOS 10.1+

``` source
class IOAudioStream : IOService
```

## Overview

An IOAudioStream represents one hardware sample buffer as well as the direction of that buffer, the mix buffer that multiple clients mix into as well as a list of all of the formats to which this buffer can be set.

When an IOAudioEngine is created during init time in the driver, an IOAudioStream must be created for each sample buffer in the device. Typically, the sample buffer will be interleaved (or single channel), as a non-interleaved buffer should be divided into multiple single-channel buffers (and multiple IOAudioStreams).

Additionally, when an IOAudioStream is created it must have all of the possible formats (and allowed sample rates for each format) set and must have the currently set format specified (addAvailableFormat() and setFormat()).

## Topics

### Instance Methods

- addAvailableFormatDeprecated

- addAvailableFormatDeprecated

- addAvailableFormatDeprecated

- addAvailableFormatDeprecated

- addClientDeprecated

- addDefaultAudioControlDeprecated

- clearAvailableFormatsDeprecated

- clearSampleBufferDeprecated

- clipIfNecessaryDeprecated

- clipOutputSamplesDeprecated

- freeDeprecated

- getDirectionDeprecated

- getFormatDeprecated

- getFormatExtensionDeprecated

- getMaxNumChannelsDeprecated

- getMetaClass

- getMixBufferDeprecated

- getMixBufferSizeDeprecated

- getNumClientsDeprecated

- getNumSampleFramesReadDeprecated

- getSampleBufferDeprecated

- getSampleBufferSizeDeprecated

- getStartingChannelIDDeprecated

- getStreamAvailableDeprecated

- getWorkLoop

- hardwareFormatChangedDeprecated

- initWithAudioEngineDeprecated

- lockStreamForIODeprecated

- mixOutputSamplesDeprecated

- numSampleFramesPerBufferChangedDeprecated

- processOutputSamplesDeprecated

- readInputSamplesDeprecated

- removeClientDeprecated

- removeDefaultAudioControlsDeprecated

- resetClipInfoDeprecated

- safeLogErrorDeprecated

- setDefaultNumSampleFramesReadDeprecated

- setDirectionDeprecated

- setFormatDeprecated

- setFormatDeprecated

- setFormatDeprecated

- setFormatDeprecated

- setFormatDeprecated

- setIOFunctionDeprecated

- setIOFunctionListDeprecated

- setMixBufferDeprecated

- setPropertiesDeprecated

- setSampleBufferDeprecated

- setSampleLatencyDeprecated

- setStartingChannelNumberDeprecated

- setStreamAvailableDeprecated

- setTerminalTypeDeprecated

- stopDeprecated

- unlockStreamForIODeprecated

- updateNumClientsDeprecated

- validateFormatDeprecated

- validateFormatDeprecated

- validateFormatDeprecated

### Type Methods

+ createDictionaryFromFormatDeprecated

+ createFormatFromDictionaryDeprecated

+ initKeysDeprecated

+ setFormatActionDeprecated

## Relationships

### Inherits From

- IOService

## See Also

### Interfaces

IOAudioLevelControl

IOAudioSelectorControl

IOAudioToggleControl

IOAudioControl

Represents any controllable attribute of an IOAudioDevice.

IOAudioEngine

Abstract base class for a single audio audio / I/O engine.

IOAudioPort

Represents a logical or physical port or functional unit in an audio device.

