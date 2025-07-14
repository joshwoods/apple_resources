

- AVFAudio
-  AVAudioSessionInterruptionWasSuspendedKey Deprecated

Global Variable

# AVAudioSessionInterruptionWasSuspendedKey

A user info key used to determine if the interruption is due to the audio session being deactivated when the system suspended the app.

iOS 10.3–14.5DeprecatediPadOS 10.3–14.5DeprecatedMac Catalyst 13.1–14.5DeprecatedmacOStvOS 10.3–14.5DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.2–7.3Deprecated

``` source
let AVAudioSessionInterruptionWasSuspendedKey: String
```

Deprecated

Use AVAudioSessionInterruptionReasonKey instead.

## Discussion

This userInfo key is present only in AVAudioSession.InterruptionType.began interruption events, where the interruption is a direct result of the operating system suspending the app. Its associated value is a Boolean NSNumber, where a true value indicates that the interruption is due to the system suspending the app, rather than being interrupted by another audio session.

## See Also

### User Info Keys

let AVAudioSessionInterruptionTypeKey: String

A user info key to retrieve the interruption type.

let AVAudioSessionInterruptionOptionKey: String

A user info key to retrieve the interruption option.

let AVAudioSessionInterruptionReasonKey: String

A user info key to retrieve the interruption reason.

