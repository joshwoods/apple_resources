

- AVFoundation
- AVSampleBufferAudioRenderer
-  audioOutputDeviceUniqueID 

Instance Property

# audioOutputDeviceUniqueID

The unique identifier of the output device used to play audio.

macOS 10.13+

``` source
var audioOutputDeviceUniqueID: String? { get set }
```

## Discussion

The default value of this property is `nil`, which indicates the use of the default audio device. Otherwise, set the value to an NSString containing the unique identifier of the Core Audio output device to use for audio output. kAudioDevicePropertyDeviceUID is a suitable source of audio output device unique IDs.

Modifying this property while the timebase’s rate isn’t `0.0` may cause the rate to briefly change to `0.0`.

On macOS, you can use the audio device clock as the AVSampleBufferRenderSynchronizer and all attached AVQueuedSampleBufferRendering timebase clocks. If you modify the `audioOutputDeviceUniqueID`, the clocks of all these timebases may also change.

If you attach multiple renderers with different values for `audioOutputDeviceUniqueID` to the same buffer renderer synchronizer, audio may not stay in sync during playback. To avoid this, ensure that all synchronized sample buffer renderers are using the same audio output device.

## See Also

### Managing Audio Output

var volume: Float

The current audio volume for the audio renderer.

var isMuted: Bool

A Boolean value that indicates whether audio for the renderer is in a muted state.

