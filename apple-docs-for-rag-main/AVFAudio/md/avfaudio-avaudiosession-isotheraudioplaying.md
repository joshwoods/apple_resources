

- AVFAudio
- AVAudioSession
-  isOtherAudioPlaying 

Instance Property

# isOtherAudioPlaying

A Boolean value that indicates whether another app is playing audio.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isOtherAudioPlaying: Bool { get }
```

## Discussion

This property returns true if any other audio is playing, including audio from an app using the ambient category. Most apps should instead use the secondaryAudioShouldBeSilencedHint property, because it’s more restrictive when considering whether primary audio from another app is playing.

## See Also

### Mixing with other audio

var secondaryAudioShouldBeSilencedHint: Bool

A Boolean value that indicates whether another app, with a nonmixable audio session, is playing audio.

class let silenceSecondaryAudioHintNotification: NSNotification.Name

A notification the system posts when the primary audio from other apps starts and stops.

var allowHapticsAndSystemSoundsDuringRecording: Bool

A Boolean value that indicates whether system sounds and haptics play while recording from audio input.

func setAllowHapticsAndSystemSoundsDuringRecording(Bool) throws

Sets a Boolean value that indicates whether system sounds and haptics play while recording from audio input.

