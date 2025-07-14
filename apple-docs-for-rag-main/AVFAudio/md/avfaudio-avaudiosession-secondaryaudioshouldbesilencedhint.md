

- AVFAudio
- AVAudioSession
-  secondaryAudioShouldBeSilencedHint 

Instance Property

# secondaryAudioShouldBeSilencedHint

A Boolean value that indicates whether another app, with a nonmixable audio session, is playing audio.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var secondaryAudioShouldBeSilencedHint: Bool { get }
```

## Discussion

Use this property as a hint to silence audio that’s secondary to the functionality of the app. For example, in a game that uses the ambient category, you can use this property to mute the soundtrack while leaving sound effects unmuted.

## See Also

### Mixing with other audio

var isOtherAudioPlaying: Bool

A Boolean value that indicates whether another app is playing audio.

class let silenceSecondaryAudioHintNotification: NSNotification.Name

A notification the system posts when the primary audio from other apps starts and stops.

var allowHapticsAndSystemSoundsDuringRecording: Bool

A Boolean value that indicates whether system sounds and haptics play while recording from audio input.

func setAllowHapticsAndSystemSoundsDuringRecording(Bool) throws

Sets a Boolean value that indicates whether system sounds and haptics play while recording from audio input.

