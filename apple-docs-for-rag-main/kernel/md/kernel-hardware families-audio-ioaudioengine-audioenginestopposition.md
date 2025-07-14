

- Kernel
- Hardware Families
- Audio
- IOAudioEngine
-  audioEngineStopPosition 

# audioEngineStopPosition

``` source
IOAudioEnginePosition audioEngineStopPosition;
```

## Overview

When all clients have disconnected, this is set to one buffer length past the current audio engine position at the time. Then when the stop position is reached, the audio engine is stopped

## See Also

### Instance Variables

workLoop

userClients

status

state

sampleRate

runEraseHead

outputStreams

numSampleFramesPerBuffer

numErasesPerBuffer

numActiveUserClients

isRegistered

inputStreams

deviceStartedAudioEngine

defaultAudioControls

configurationChangeInProgress

commandGate

audioDevice

