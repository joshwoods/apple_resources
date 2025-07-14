

- Audio Toolbox
-  kAudioUnitProperty_AudioChannelLayout 

Global Variable

# kAudioUnitProperty_AudioChannelLayout

A read/write `AudioChannelLayout` data structure valid on the audio unit input and output scopes.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioUnitProperty_AudioChannelLayout: AudioUnitPropertyID { get }
```

## Discussion

The channel order, within a given audio stream, for a specified audio unit element and scope. The number of channels in the layout must match the number of channels set for the scope-element. Each input and output bus in an audio unit can have one instance of this property.

Some audio units require this property. For example, the 3DMixer unit must implement this property on its output bus. If a host application attempts to clear the value of this property on a bus that requires a valid value, the audio unit will return a kAudioUnitErr_InvalidPropertyValue error.

Input and output buses can be in one of three states in regard to Audio channel layout:

1.  Implemented and set

2.  Implemented but not set

3.  Unimplemented

Requesting the value of this property when it is implemented but not set results in a kAudioUnitErr_PropertyNotInUse error.

Use the `kAudioUnitProperty_AudioChannelLayout` property whenever channel layout is relevant.

For related information, refer to the descriptions for the `ScheduledAudioFileRegion` and AudioOutputUnitStartAtTimeParams data structures.

## See Also

### Properties

var kAudioUnitProperty_ElementCount: AudioUnitPropertyID

A read/write `UInt32` value valid on any audio unit scope. The global audio unit scope always has an element count of 1.

var kAudioUnitProperty_SupportedNumChannels: AudioUnitPropertyID

A read-only array of channel information structures valid on the audio unit global scope.

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

