

- AVFAudio
- AVAudioSession
-  setAllowHapticsAndSystemSoundsDuringRecording(\_:) 

Instance Method

# setAllowHapticsAndSystemSoundsDuringRecording(\_:)

Sets a Boolean value that indicates whether system sounds and haptics play while recording from audio input.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func setAllowHapticsAndSystemSoundsDuringRecording(_ inValue: Bool) throws
```

## Parameters 

`inValue`  

A Boolean value that indicates whether haptics and system sounds should play while recording is in progress.

## See Also

### Mixing with other audio

var isOtherAudioPlaying: Bool

A Boolean value that indicates whether another app is playing audio.

var secondaryAudioShouldBeSilencedHint: Bool

A Boolean value that indicates whether another app, with a nonmixable audio session, is playing audio.

class let silenceSecondaryAudioHintNotification: NSNotification.Name

A notification the system posts when the primary audio from other apps starts and stops.

var allowHapticsAndSystemSoundsDuringRecording: Bool

A Boolean value that indicates whether system sounds and haptics play while recording from audio input.

