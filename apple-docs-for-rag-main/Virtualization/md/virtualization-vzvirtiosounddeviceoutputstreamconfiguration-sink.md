

- Virtualization
- VZVirtioSoundDeviceOutputStreamConfiguration
-  sink 

Instance Property

# sink

An audio stream sink that defines how the host handles audio data produced by the guest.

macOS 12.0+

``` source
var sink: VZAudioOutputStreamSink? { get set }
```

## Discussion

Not specifying a sink results in a default handler that suppresses the audio. The default is `nil`.

## See Also

### Related Documentation

class VZAudioOutputStreamSink

The base class for an audio output stream sink.

class VZHostAudioOutputStreamSink

Host audio output stream sink plays audio to the host system’s default output device.

