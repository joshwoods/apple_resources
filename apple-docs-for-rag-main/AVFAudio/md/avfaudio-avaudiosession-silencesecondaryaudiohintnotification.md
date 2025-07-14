

- AVFAudio
- AVAudioSession
-  silenceSecondaryAudioHintNotification 

Type Property

# silenceSecondaryAudioHintNotification

A notification the system posts when the primary audio from other apps starts and stops.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class let silenceSecondaryAudioHintNotification: NSNotification.Name
```

## Discussion

Subscribe to this notification to ensure that the system notifies your app when optional secondary audio muting should begin or end. The system sends this notification only to registered listeners who are currently in the foreground and have an active audio session.

This notification’s userInfo dictionary contains a AVAudioSession.SilenceSecondaryAudioHintType value for the AVAudioSessionSilenceSecondaryAudioHintTypeKey. Use the audio hint type to determine if your secondary audio muting should begin or end.

```
func handleSecondaryAudio(notification: Notification) {
    // Determine hint type
    guard let userInfo = notification.userInfo,
        let typeValue = userInfo[AVAudioSessionSilenceSecondaryAudioHintTypeKey] as? UInt,
        let type = AVAudioSession.SilenceSecondaryAudioHintType(rawValue: typeValue) else {
            return
    }

    if type == .begin {
        // Other app audio started playing - mute secondary audio.
    } else {
        // Other app audio stopped playing - restart secondary audio.
    }
}
```

The system posts this notification on the main thread.

## Topics

### User Info Keys

let AVAudioSessionSilenceSecondaryAudioHintTypeKey: String

A user info key that you use to retrieve the silence secondary audio hint type.

### User Info Values

enum SilenceSecondaryAudioHintType

Constants that indicate whether optional secondary audio muting should begin or end.

## See Also

### Mixing with other audio

var isOtherAudioPlaying: Bool

A Boolean value that indicates whether another app is playing audio.

var secondaryAudioShouldBeSilencedHint: Bool

A Boolean value that indicates whether another app, with a nonmixable audio session, is playing audio.

var allowHapticsAndSystemSoundsDuringRecording: Bool

A Boolean value that indicates whether system sounds and haptics play while recording from audio input.

func setAllowHapticsAndSystemSoundsDuringRecording(Bool) throws

Sets a Boolean value that indicates whether system sounds and haptics play while recording from audio input.

