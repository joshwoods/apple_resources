

- Audio Toolbox
-  AudioUnitGetPropertyInfoProc 

Type Alias

# AudioUnitGetPropertyInfoProc

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioUnitGetPropertyInfoProc = (UnsafeMutableRawPointer, AudioUnitPropertyID, AudioUnitScope, AudioUnitElement, UnsafeMutablePointer?, UnsafeMutablePointer?) -> OSStatus
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

