

- Audio Toolbox
-  AUInputHandler 

Type Alias

# AUInputHandler

A block to notify the host of an I/O unit that an input is available.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AUInputHandler = (UnsafeMutablePointer, UnsafePointer, AUAudioFrameCount, Int) -> Void
```

## Discussion

The block takes the following parameters:

actionFlags  
The pointer to the action flags.

timestamp  
The HAL time at which the input data will be rendered. If there is a sample rate conversion or time compression/expansion downstream, the sample time will not be valid.

frameCount  
The number of sample frames of input available.

inputBusNumber  
The index of the input bus from which input is available.

The input data is obtained by calling the render block of the audio unit. The audio unit is not provided since it is not safe to message an Objective-C object in a real-time context.

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

