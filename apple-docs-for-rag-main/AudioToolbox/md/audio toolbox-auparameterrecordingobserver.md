

- Audio Toolbox
-  AUParameterRecordingObserver 

Type Alias

# AUParameterRecordingObserver

A block called to record parameter changes as automation events.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AUParameterRecordingObserver = (Int, UnsafePointer) -> Void
```

## Discussion

The block takes the following parameters:

numberEvents  
The number of events being delivered.

events  
The events being delivered.

## See Also

### Related Documentation

func token(byAddingParameterRecordingObserver: AUParameterRecordingObserver) -> AUParameterObserverToken

Adds a recording observer for a single parameter or all parameters in a group.

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

