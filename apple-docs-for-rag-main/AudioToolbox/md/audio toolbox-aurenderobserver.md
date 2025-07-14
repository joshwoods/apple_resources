

- Audio Toolbox
-  AURenderObserver 

Type Alias

# AURenderObserver

A block called when an audio unit renders audio.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AURenderObserver = (AudioUnitRenderActionFlags, UnsafePointer, AUAudioFrameCount, Int) -> Void
```

## Discussion

This block is called by the base class’s AURenderBlock block before and after each render cycle. The observer can distinguish between before and after using the unitRenderAction_PreRender and unitRenderAction_PostRender action flag values.

The block takes the following parameters:

actionFlags  
The pointer to the action flags.

timestamp  
The HAL time at which the input data will be rendered. If there is a sample rate conversion or time compression/expansion downstream, the sample time will not have a defined correlation with the `AudioDevice` sample time.

frameCount  
The number of sample frames to render.

outputBusNumber  
The index of the output bus to render.

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

