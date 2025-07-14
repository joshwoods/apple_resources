

- Audio Toolbox
-  AudioUnitPropertyListenerProc 

Type Alias

# AudioUnitPropertyListenerProc

Called by the system when the value of a specified audio unit property has changed.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioUnitPropertyListenerProc = (UnsafeMutableRawPointer, AudioUnit, AudioUnitPropertyID, AudioUnitScope, AudioUnitElement) -> Void
```

## Parameters 

`inRefCon`  

Custom data that you provided when registering your callback with the audio unit.

`inUnit`  

The audio unit upon which the specified property value has changed.

`inID`  

The property whose value has changed.

`inScope`  

The scope of the property whose value has changed.

`inElement`  

The element ID on the scope of the property whose value has changed.

## Return Value

A result code.

## Discussion

If you named your callback function `MyAudioUnitPropertyListenerProc`, you would declare it like this:

### Discussion

You register your `AudioUnitPropertyListenerProc` callback function using the AudioUnitAddPropertyListener(_:_:_:_:) function.

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

