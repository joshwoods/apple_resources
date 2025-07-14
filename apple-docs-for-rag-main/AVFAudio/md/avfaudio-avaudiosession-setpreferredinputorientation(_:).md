

- AVFAudio
- AVAudioSession
-  setPreferredInputOrientation(\_:) 

Instance Method

# setPreferredInputOrientation(\_:)

Sets the audio session’s preferred stereo input orientation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func setPreferredInputOrientation(_ orientation: AVAudioSession.StereoOrientation) throws
```

## Parameters 

`orientation`  

The stereo orientation.

## Discussion

Configure the input orientation to match how the user is holding the device when they begin recording. In a single-window app, set the input orientation to a value corresponding to the app’s user interface orientation.

## See Also

### Enabling stereo recording

var inputOrientation: AVAudioSession.StereoOrientation

An orientation value that dictates which directions represent left and right when capturing audio from a built-in microphone configured for stereo recording.

var preferredInputOrientation: AVAudioSession.StereoOrientation

The audio session’s preferred stereo input orientation.

enum StereoOrientation

Constants that define the supported stereo orientations.

