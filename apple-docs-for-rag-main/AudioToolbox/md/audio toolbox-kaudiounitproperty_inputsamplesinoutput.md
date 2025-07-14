

- Audio Toolbox
-  kAudioUnitProperty_InputSamplesInOutput 

Global Variable

# kAudioUnitProperty_InputSamplesInOutput

A read/write AUInputSamplesInOutputCallbackStruct struct, valid on the audio unit global scope.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioUnitProperty_InputSamplesInOutput: AudioUnitPropertyID { get }
```

## Discussion

An audio unit calls this callback at the end of its render call. The audio unit supplies the following information:

- outputTime - The timestamp passed in to the audio unit’s render call. This timestamp represents the time of the first output sample.

- inputSample - The sample number of the first input sample that is present in the output audio.

- numInputSamples - The number of input samples that were used and are present in the output audio.

This property allows a host application to determine which input samples correspond to a sample in the output buffer. It is useful only for audio units that do time-stretching, such as the macOS AUVaripseed and AUTimePitch units, where the relationship between input and output samples is non-trivial. For these units, the range of input samples that correspond to an output buffer typically differs from the range of input samples that were pulled for that render call. This difference arises because of internal buffering, processing latency, and other factors.

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

