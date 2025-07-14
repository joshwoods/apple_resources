

- Audio Toolbox
-  kAudioUnitProperty_MIDIOutputCallback 

Global Variable

# kAudioUnitProperty_MIDIOutputCallback

A write-only AUMIDIOutputCallbackStruct struct, valid on the audio unit global scope.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioUnitProperty_MIDIOutputCallback: AudioUnitPropertyID { get }
```

## Discussion

The host sets this property on the audio unit with the callback (and its user data) set appropriately.

Operational Parameters: In the render call, just as is the expected usage of the AUHostCallbacks, the audio unit can call the provided callback to provide MIDI data to the host that it will associate with the current AudioUnitRender call in process.

The audio unit in the callback provides the following:

- the user data provided by the host when the callback was established

- the AudioTimeStamp that was provided to the audio unit for this particular call of AudioUnitRender

- the output number to associate this MIDI data with

- a MIDI Packet List containing MIDI data. The time stamp values contained within the MIDIPackets in this list are \*\*sample offsets\*\*\* from the AudioTimeStamp provided

This allows MIDI data to be time-stamped with a sample offset that is directly associated with the audio data it is generating in the current call to the AudioUnitRender function.

There is no implied or expected association between the number (or position) of an audio unit’s audio or MIDI outputs.

## See Also

### Properties

var kAudioUnitProperty_ElementCount: AudioUnitPropertyID

A read/write `UInt32` value valid on any audio unit scope. The global audio unit scope always has an element count of 1.

var kAudioUnitProperty_SupportedNumChannels: AudioUnitPropertyID

A read-only array of channel information structures valid on the audio unit global scope.

var kAudioUnitProperty_AudioChannelLayout: AudioUnitPropertyID

A read/write `AudioChannelLayout` data structure valid on the audio unit input and output scopes.

var kAudioUnitProperty_AudioUnitMIDIProtocol: AudioUnitPropertyID

var kAudioUnitProperty_AUHostIdentifier: AudioUnitPropertyID

var kAudioUnitProperty_BypassEffect: AudioUnitPropertyID

A read/write `UInt32` value, representing a Boolean value, valid on the audio unit global scope.

var kAudioUnitProperty_ClassInfo: AudioUnitPropertyID

Describes the state of an audio unit.

var kAudioUnitProperty_ClassInfoFromDocument: AudioUnitPropertyID

A read/write CFDictionary object, valid on the audio unit global scope.

var kAudioUnitProperty_CocoaUI: AudioUnitPropertyID

A read-only `AudioUnitCocoaViewInfo` data structure valid on the audio unit global scope.

var kAudioUnitProperty_ContextName: AudioUnitPropertyID

var kAudioUnitProperty_CPULoad: AudioUnitPropertyID

A read-only `Float64` value valid on the audio unit global scope.

var kAudioUnitProperty_DependentParameters: AudioUnitPropertyID

var kAudioUnitProperty_ElementName: AudioUnitPropertyID

The name of the specified element.

var kAudioUnitProperty_FactoryPresets: AudioUnitPropertyID

So-called *factory presets* (as opposed to user-configured presets) are ones supplied with an audio unit by the manufacturer. You choose the active preset by setting the `kAudioUnitProperty_PresentPreset` property.

var kAudioUnitProperty_FastDispatch: AudioUnitPropertyID

A read-only `void *` value valid on the audio unit global scope.

