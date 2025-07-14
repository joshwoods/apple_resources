

- Audio Toolbox
-  AUImplementorValueProvider 

Type Alias

# AUImplementorValueProvider

A block called to fetch a parameter’s current value from the audio unit implementation.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AUImplementorValueProvider = (AUParameter) -> AUValue
```

## Discussion

This block is only of interest to audio unit subclasses.

The block returns the current value of the parameter.

The block takes the following parameters:

param  
The parameter to query.

## See Also

### Related Documentation

var implementorValueProvider: AUImplementorValueProvider

The callback for refreshing known stale values in a parameter tree.

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

typealias AUInputHandler

A block to notify the host of an I/O unit that an input is available.

