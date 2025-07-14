

- AVFoundation
- AVPlayer
-  audioOutputDeviceUniqueID 

Instance Property

# audioOutputDeviceUniqueID

Specifies the unique ID of the Core Audio output device used to play audio.

macOS 10.9+

``` source
nonisolated
var audioOutputDeviceUniqueID: String? { get set }
```

## Discussion

The default value of this property is `nil`, indicating that the default audio output device is used. Otherwise the value of this property is a string containing the unique ID of the Core Audio output device to be used for audio output.

Core Audio’s kAudioDevicePropertyDeviceUID is a suitable source of audio output device unique IDs.

## See Also

### Configuring Audio and Video Devices

var preferredVideoDecoderGPURegistryID: UInt64

The registry identifier for the GPU used for video decoding.

