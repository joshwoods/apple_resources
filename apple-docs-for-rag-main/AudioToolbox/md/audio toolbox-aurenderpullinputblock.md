

- Audio Toolbox
-  AURenderPullInputBlock 

Type Alias

# AURenderPullInputBlock

A block to supply audio input to a render block.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AURenderPullInputBlock = (UnsafeMutablePointer, UnsafePointer, AUAudioFrameCount, Int, UnsafeMutablePointer) -> AUAudioUnitStatus
```

## Discussion

The caller must supply valid buffers in the input data’s `mBuffers'` `mData` and `mDataByteSize` fields (`mDataByteSize` must be consistent with `frameCount`). This block may provide input in those specified buffers, or it may replace the `mData` pointers with pointers to memory which it owns and guarantees will remain valid until the next render cycle.

The block returns an audio unit status result code. If instead an error is returned, the input data should be assumed to be invalid.

The block takes the following parameters:

actionFlags  
The pointer to the action flags.

timestamp  
The HAL time at which the input data will be rendered. If there is a sample rate conversion or time compression/expansion downstream, the sample time will not be valid.

frameCount  
The number of input sample frames requested.

inputBusNumber  
The index of the input bus being pulled.

inputData  
The input audio data.

## See Also

### Audio Unit Types

struct ScheduledAudioFileRegion

struct ScheduledAudioSlice

typealias ScheduledAudioFileRegionCompletionProc

typealias ScheduledAudioSliceCompletionProc

typealias MIDIChannelNumber

MIDI Channel, 0~15 (channels 1 through 16, respectively).

typealias AUAudioObjectID

typealias AUMIDICIProfileChangedBlock

typealias AUAudioChannelCount

A number of audio channels.

typealias AUAudioFrameCount

A number of audio sample frames.

typealias AUAudioUnitStatus

A result code returned from an audio unit’s render function.

typealias AUEventListenerProc

typealias AUEventListenerRef

typealias AUEventSampleTime

Expresses time as a sample count.

typealias AUImplementorValueObserver

A block called to notify the audio unit implementation of changes to a parameter value.

typealias AUImplementorValueProvider

A block called to fetch a parameter’s current value from the audio unit implementation.

