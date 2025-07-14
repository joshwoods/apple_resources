

- Virtualization
- VZVirtioSoundDeviceInputStreamConfiguration
-  source 

Instance Property

# source

An audio stream source that defines how the host supplies audio data for the guest.

macOS 12.0+

``` source
var source: VZAudioInputStreamSource? { get set }
```

## Discussion

Not specifying a source results in a default handler that produces audio silence. The default is `nil`.

## See Also

### Related Documentation

class VZAudioInputStreamSource

The base class for an audio input stream source.

class VZHostAudioInputStreamSource

The host audio input stream source that provides audio from the host system’s default input device.

