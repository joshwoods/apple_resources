

- Audio Toolbox
-  AUImplementorValueObserver 

Type Alias

# AUImplementorValueObserver

A block called to notify the audio unit implementation of changes to a parameter value.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AUImplementorValueObserver = (AUParameter, AUValue) -> Void
```

## Discussion

This block is only of interest to audio unit subclasses.

The block takes the following parameters:

param  
The parameter that was changed.

value  
The current value of the parameter.

## See Also

### Related Documentation

var implementorValueObserver: AUImplementorValueObserver

The callback for parameter value changes.

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

typealias AUImplementorValueProvider

A block called to fetch a parameter’s current value from the audio unit implementation.

typealias AUInputHandler

A block to notify the host of an I/O unit that an input is available.

