

- AVFAudio
- AVAudioSession
-  inputOrientation 

Instance Property

# inputOrientation

An orientation value that dictates which directions represent left and right when capturing audio from a built-in microphone configured for stereo recording.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var inputOrientation: AVAudioSession.StereoOrientation { get }
```

## Discussion

If you’re recording video, set the input orientation to match the video orientation. If you’re recording audio only, set the input orientation to match the user interface orientation. In either case, don’t modify the input orientation during recording.

Important

The audio session’s input orientation is independent of the orientation property of an AVAudioSessionDataSourceDescription.

## See Also

### Enabling stereo recording

var preferredInputOrientation: AVAudioSession.StereoOrientation

The audio session’s preferred stereo input orientation.

func setPreferredInputOrientation(AVAudioSession.StereoOrientation) throws

Sets the audio session’s preferred stereo input orientation.

enum StereoOrientation

Constants that define the supported stereo orientations.

