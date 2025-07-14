

- Audio Toolbox
-  kAudioUnitProperty_MaximumFramesPerSlice 

Global Variable

# kAudioUnitProperty_MaximumFramesPerSlice

Specifies the maximum number of sample frames an audio unit is prepared to supply on one invocation of its AudioUnitRender(_:_:_:_:_:_:) function.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioUnitProperty_MaximumFramesPerSlice: AudioUnitPropertyID { get }
```

## Discussion

A read/write `UInt32` value valid on the audio unit global scope.

The default value of this property is 1,024, corresponding to about 23 ms at a 44.1 kHz sample rate. This default value is sufficient when a host app is using the default hardware buffer size and the device screen is not sleeping. When the device screen sleeps, the system saves power by reducing the frequency at which it requests sample frames. There is a corresponding increase in the number of sample frames requested of an audio unit, per render call.

The following table provides some common slice sizes:

|              | Frame count | Milliseconds at 44.1 kHz (approximate) |
|--------------|-------------|----------------------------------------|
| Default      | 1024        | 23                                     |
| Screen sleep | 4096        | 93                                     |
| Low latency  | 256         | 5                                      |

You never need to set this property for I/O units because they are preconfigured to handle any slice size requested by the system. For all other audio units, you must set this property to a value of 4096 to handle screen sleep—unless audio input is running on the device. When audio input is running, the system maintains a slice size of 1024.

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

