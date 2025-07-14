

- Audio Toolbox
-  kAudioUnitProperty_ParameterValueStrings 

Global Variable

# kAudioUnitProperty_ParameterValueStrings

An array of names for a named, indexed audio unit parameter. An indexed parameter is one whose unit type is AudioUnitParameterUnit.indexed. The array’s strings can be used to build a menu for the parameter.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioUnitProperty_ParameterValueStrings: AudioUnitPropertyID { get }
```

## Discussion

A read-only CFArray object whose elements are CFString objects, valid on any audio unit scope.

When obtaining a parameter string array from an audio unit with the AudioUnitGetProperty(_:_:_:_:_:_:) function, you own the reference to the array and are responsible for later releasing it by calling the CFRelease function.

Indexed parameters use whole-number index values; the size of this property’s array should be the same as the range between the parameter’s minimum and maximum values.

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

