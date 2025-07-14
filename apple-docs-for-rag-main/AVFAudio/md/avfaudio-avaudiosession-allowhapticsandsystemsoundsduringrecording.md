

- AVFAudio
- AVAudioSession
-  allowHapticsAndSystemSoundsDuringRecording 

Instance Property

# allowHapticsAndSystemSoundsDuringRecording

A Boolean value that indicates whether system sounds and haptics play while recording from audio input.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var allowHapticsAndSystemSoundsDuringRecording: Bool { get }
```

## Discussion

The default value of this property is false.

## See Also

### Mixing with other audio

var isOtherAudioPlaying: Bool

A Boolean value that indicates whether another app is playing audio.

var secondaryAudioShouldBeSilencedHint: Bool

A Boolean value that indicates whether another app, with a nonmixable audio session, is playing audio.

class let silenceSecondaryAudioHintNotification: NSNotification.Name

A notification the system posts when the primary audio from other apps starts and stops.

func setAllowHapticsAndSystemSoundsDuringRecording(Bool) throws

Sets a Boolean value that indicates whether system sounds and haptics play while recording from audio input.

