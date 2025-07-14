

- Audio Toolbox
-  AURenderBlock 

Type Alias

# AURenderBlock

A block to render the audio unit.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AURenderBlock = (UnsafeMutablePointer, UnsafePointer, AUAudioFrameCount, Int, UnsafeMutablePointer, AURenderPullInputBlock?) -> AUAudioUnitStatus
```

## Discussion

All realtime operations are implemented using blocks to avoid Objective-C method dispatching and the possibility of blocking.

The block returns an audio unit status result code. If instead an error is returned, the output data should be assumed to be invalid.

The block takes the following parameters:

actionFlags  
The pointer to the action flags.

timestamp  
The HAL time at which the input data will be rendered. If there is a sample rate conversion or time compression/expansion downstream, the sample time will not have a defined correlation with the `AudioDevice` sample time.

frameCount  
The number of sample frames to render.

outputBusNumber  
The index of the output bus to render.

outputData  
The output bus’s render buffers and flags. The buffer pointers may be null on entry, in which case the block will render into memory it owns and modify the `mData` pointers to point to that memory. The block is responsible for preserving the validity of that memory until it is next called to render, or until the deallocateRenderResources() method is called.

pullInputBlock  
A block that the audio unit will call in order to pull for input data. This value may be `nil` for instrument and audio generator units (which do not have input busses).

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

