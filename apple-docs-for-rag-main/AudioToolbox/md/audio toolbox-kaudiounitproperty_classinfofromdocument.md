

- Audio Toolbox
-  kAudioUnitProperty_ClassInfoFromDocument 

Global Variable

# kAudioUnitProperty_ClassInfoFromDocument

A read/write CFDictionary object, valid on the audio unit global scope.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioUnitProperty_ClassInfoFromDocument: AudioUnitPropertyID { get }
```

## Discussion

If the audio unit implements this property then it is going to do different actions establishing its state from a document rather than from a user preset. Thus, a host app should use this property first (instead of kAudioUnitProperty_ClassInfo) when restoring the state of an audio unit when opening a document. If the audio unit returns an error (or doesn’t implement this property) then the host should use the same preset with the kAudioUnitProperty_ClassInfo.

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

