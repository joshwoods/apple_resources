

- AVFAudio
-  AVAudioSessionInterruptionOptionKey 

Global Variable

# AVAudioSessionInterruptionOptionKey

A user info key to retrieve the interruption option.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let AVAudioSessionInterruptionOptionKey: String
```

## Discussion

The value for this key is an NSNumber object containing an unsigned integer that identifies any options associated with the interruption. For a list of possible flags, see AVAudioSession.InterruptionOptions.

## See Also

### User Info Keys

let AVAudioSessionInterruptionTypeKey: String

A user info key to retrieve the interruption type.

let AVAudioSessionInterruptionReasonKey: String

A user info key to retrieve the interruption reason.

let AVAudioSessionInterruptionWasSuspendedKey: String

A user info key used to determine if the interruption is due to the audio session being deactivated when the system suspended the app.

Deprecated

