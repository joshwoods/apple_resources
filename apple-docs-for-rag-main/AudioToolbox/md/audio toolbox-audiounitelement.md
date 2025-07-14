

- Audio Toolbox
-  AudioUnitElement 

Type Alias

# AudioUnitElement

The data type for an audio unit element identifier.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioUnitElement = UInt32
```

## Discussion

An audio unit element is a discrete programmatic context that is nested within an audio unit scope (see AudioUnitScope). In the context of input and output scopes, elements serve as programmatic analogs of physical signal buses in hardware audio devices. Because of this analogy, the term “bus” is a common synonym for “element.”

Elements are zero indexed. The Global scope always has exactly one element—element 0.

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

