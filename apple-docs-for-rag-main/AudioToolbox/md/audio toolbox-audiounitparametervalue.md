

- Audio Toolbox
-  AudioUnitParameterValue 

Type Alias

# AudioUnitParameterValue

The data type for an audio unit parameter value.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioUnitParameterValue = Float32
```

## Discussion

An audio unit parameter is an adjustable setting, such as gain. The parameters for Apple-supplied audio units are described in `Audio Unit Parameters`.

You can change a parameter value directly by calling the AudioUnitSetParameter(_:_:_:_:_:_:) function, or schedule a change by calling AudioUnitScheduleParameters(_:_:_:). See also AudioUnitParameterID, AudioUnitParameter.

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

