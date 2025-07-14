

- AVFAudio
- AVAudioSession
-  setAggregatedIOPreference(\_:) 

Instance Method

# setAggregatedIOPreference(\_:)

Sets the audio session’s aggregated I/O configuration preference.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setAggregatedIOPreference(_ inIOType: AVAudioSession.IOType) throws
```

## Parameters 

`inIOType`  

The aggregated I/O preference that you want to use.

## Discussion

Starting with iOS 10, AVCaptureSession has changed its default audio input configuration on iPhone and iPad devices that support the Live Photos feature. This change allows taking a Live Photo without interrupting background audio playback. Configure your preferred audio input behavior by setting your aggregated I/O preference.

Apps that use AVCaptureSession in its default audio input configuration (usesApplicationAudioSession `=` true, automaticallyConfiguresApplicationAudioSession `=` true), and that need to guarantee the same behavior as previous versions of iOS, should opt-out of this new behavior by setting the aggregated I/O preference to AVAudioSession.IOType.aggregated.

Apps that don’t use AVCaptureSession, or that use a capture session in its nondefault configuration, can ignore this preference. In these cases, there’s no change in behavior from previous versions of iOS.

## See Also

### Setting the aggregated I/O preference

enum IOType

Constant values used to specify the audio session’s aggregated I/O behavior.

