

- AVFoundation
- AVSampleBufferAudioRenderer
-  volume 

Instance Property

# volume

The current audio volume for the audio renderer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var volume: Float { get set }
```

## Discussion

Use this property for frequent vloume changes; for example, a volume knob or fader. A value of `0.0` silences all audio while a value of `1.0` plays all audio at full volume.

## See Also

### Managing Audio Output

var isMuted: Bool

A Boolean value that indicates whether audio for the renderer is in a muted state.

var audioOutputDeviceUniqueID: String?

The unique identifier of the output device used to play audio.

