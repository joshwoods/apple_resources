

- Audio Toolbox
-  kAudioUnitProperty_FastDispatch 

Global Variable

# kAudioUnitProperty_FastDispatch

A read-only `void *` value valid on the audio unit global scope.

macOS

``` source
var kAudioUnitProperty_FastDispatch: AudioUnitPropertyID { get }
```

## Discussion

This property supports expedited interaction with an audio unit. To use it, call the AudioUnitGetProperty(_:_:_:_:_:_:) function with the `inID` parameter set to the selector constant that corresponds to the audio unit function you want to call quickly. On return, the `outData` parameter contains a function pointer for the selector.

For example, by calling AudioUnitGetProperty(_:_:_:_:_:_:) with its `inID` parameter set to `kAudioUnitRenderSelect`, you obtain the function pointer for the AudioUnitRender(_:_:_:_:_:_:) function. You can then invoke audio unit rendering without incurring the overhead of the component dispatch mechanism.

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

var kAudioUnitProperty_FrequencyResponse: AudioUnitPropertyID

