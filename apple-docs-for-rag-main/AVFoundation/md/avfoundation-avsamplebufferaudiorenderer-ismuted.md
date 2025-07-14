

- AVFoundation
- AVSampleBufferAudioRenderer
-  isMuted 

Instance Property

# isMuted

A Boolean value that indicates whether audio for the renderer is in a muted state.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var isMuted: Bool { get set }
```

## Discussion

This property only affects muting the renderer instance and not the device.

## See Also

### Managing Audio Output

var volume: Float

The current audio volume for the audio renderer.

var audioOutputDeviceUniqueID: String?

The unique identifier of the output device used to play audio.

