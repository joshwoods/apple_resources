

- Audio Toolbox
-  AUParameterObserver 

Type Alias

# AUParameterObserver

A block called after the value of a parameter changes.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AUParameterObserver = (AUParameterAddress, AUValue) -> Void
```

## Discussion

The block takes the following parameters:

address  
The address of the parameter.

value  
The current value of the parameter.

## See Also

### Related Documentation

func token(byAddingParameterObserver: AUParameterObserver) -> AUParameterObserverToken

Adds an observer for a single parameter or all parameters in a group.

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

