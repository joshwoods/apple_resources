

- Audio Toolbox
-  kAudioUnitProperty_ShouldAllocateBuffer 

Global Variable

# kAudioUnitProperty_ShouldAllocateBuffer

A read/write `UInt32` value valid on the audio unit input and output scopes, settable individually on each element.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioUnitProperty_ShouldAllocateBuffer: AudioUnitPropertyID { get }
```

## Discussion

Default value is `true`, which means that the associated audio unit element creates a buffer for rendering into.

If true, the element will create a buffer for rendering into.

If false, the element will not create a buffer for rendering.

For example, if the audio unit is only ever going to have a connection as its input and never a callback, then it should not need to create a buffer (the API contract expects an audio unit to provide a buffer for callbacks, but no buffer for connections).

If the audio unit is always going to be pulled for audio with the client providing audio data buffers to the AudioUnitRender call, then it will never need to create an audio buffer on the output side.

So, this property can be used to control the default allocation strategy of an audio unit. If the audio unit needs a buffer, but one hasn’t been allocated, then an error will be thrown from that call to AudioUnitRender.

This property cannot be set on initialized audio units as it may end up reallocating memory.

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

