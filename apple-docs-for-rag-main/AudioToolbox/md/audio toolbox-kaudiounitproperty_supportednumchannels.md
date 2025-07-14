

- Audio Toolbox
-  kAudioUnitProperty_SupportedNumChannels 

Global Variable

# kAudioUnitProperty_SupportedNumChannels

A read-only array of channel information structures valid on the audio unit global scope.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioUnitProperty_SupportedNumChannels: AudioUnitPropertyID { get }
```

## Discussion

The size of the array indicates the number of AUChannelInfo structures for an audio unit. Each structure describes the channel configuration for an audio input/output bus. For example, the values (2, 2) indicates a channel configuration of two input channels paired to two output channels on a bus.

A negative value for a field in an AUChannelInfo structure indicates that an input/output bus supports a variable number of channels, as follows:

- {–1, –1} indicates that a bus supports any number of input or output channels provided that the input and output channel counts match each other. This is the default configuration for effect units.

- {–1, –2} or {–2, –1} indicates that a bus supports any number of input and output channels; the channel counts on input and output can differ from each other.

- {–1, –3} indicates that a bus supports any number of input channels and up to three output channels.

A value of 0 for the `inChannels` field means that an audio unit does not have any audio input buses.

## See Also

### Properties

var kAudioUnitProperty_ElementCount: AudioUnitPropertyID

A read/write `UInt32` value valid on any audio unit scope. The global audio unit scope always has an element count of 1.

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

var kAudioUnitProperty_FrequencyResponse: AudioUnitPropertyID

