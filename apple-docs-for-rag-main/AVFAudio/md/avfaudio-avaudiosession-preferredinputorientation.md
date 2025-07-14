

- AVFAudio
- AVAudioSession
-  preferredInputOrientation 

Instance Property

# preferredInputOrientation

The audio session’s preferred stereo input orientation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var preferredInputOrientation: AVAudioSession.StereoOrientation { get }
```

## See Also

### Enabling stereo recording

var inputOrientation: AVAudioSession.StereoOrientation

An orientation value that dictates which directions represent left and right when capturing audio from a built-in microphone configured for stereo recording.

func setPreferredInputOrientation(AVAudioSession.StereoOrientation) throws

Sets the audio session’s preferred stereo input orientation.

enum StereoOrientation

Constants that define the supported stereo orientations.

