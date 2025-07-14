

- AVFAudio
-  AVAudioSessionInterruptionTypeKey 

Global Variable

# AVAudioSessionInterruptionTypeKey

A user info key to retrieve the interruption type.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let AVAudioSessionInterruptionTypeKey: String
```

## Discussion

The value for this key is an NSNumber object containing an unsigned integer that identifies the type of interruption. For a list of possible values, see AVAudioSession.InterruptionType.

## See Also

### User Info Keys

let AVAudioSessionInterruptionOptionKey: String

A user info key to retrieve the interruption option.

let AVAudioSessionInterruptionReasonKey: String

A user info key to retrieve the interruption reason.

let AVAudioSessionInterruptionWasSuspendedKey: String

A user info key used to determine if the interruption is due to the audio session being deactivated when the system suspended the app.

Deprecated

