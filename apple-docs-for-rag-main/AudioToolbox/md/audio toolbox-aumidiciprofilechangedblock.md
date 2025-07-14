

- Audio Toolbox
-  AUMIDICIProfileChangedBlock 

Type Alias

# AUMIDICIProfileChangedBlock

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+

``` source
typealias AUMIDICIProfileChangedBlock = (UInt8, MIDIChannelNumber, MIDICIProfile, Bool) -> Void
```

## See Also

### Audio Unit Types

struct ScheduledAudioFileRegion

struct ScheduledAudioSlice

typealias ScheduledAudioFileRegionCompletionProc

typealias ScheduledAudioSliceCompletionProc

typealias MIDIChannelNumber

MIDI Channel, 0~15 (channels 1 through 16, respectively).

typealias AUAudioObjectID

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

typealias AUInputHandler

A block to notify the host of an I/O unit that an input is available.

