

- Audio Toolbox
-  kAudioUnitProperty_SupportedChannelLayoutTags 

Global Variable

# kAudioUnitProperty_SupportedChannelLayoutTags

A read-only array on `AudioChannelLayoutTag` structures, valid on the audio unit input and output scopes.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioUnitProperty_SupportedChannelLayoutTags: AudioUnitPropertyID { get }
```

## Discussion

Used with GetProperty to ascertain what an audio unit understands about laying out of channel orders. This will typically return one or more of the specified layout tags.

When a specific set of layouts are returned, the client then uses the kAudioUnitProperty_AudioChannelLayout property (with one of those layout tags specified) to set the unit to use that layout. In this case the client (and the audio unit when reporting its AudioChannelLayout) is only expected to have set an AudioChannelLayout which only sets the layout tag as the valid field.

Some audio units may return the tag `kAudioChannelLayoutTag_UseChannelDescriptions`. This indicates a custom channel map.

In this case, the host then can look at supported number of channels on that scope (using the kAudioUnitProperty_SupportedNumChannels), and supply an AudioChannelLayout with the kAudioUnitProperty_AudioChannelLayout property to specify the layout, number of channels and location of each of those channels. This custom channel map MUST have a channel valence that is supported by the Audio Unit.

The UseChannelBitmap field is NOT used within the context of the AudioUnit.

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

