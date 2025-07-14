

- AVFAudio
- AVAudioSession
-  interruptionNotification 

Type Property

# interruptionNotification

A notification the system posts when an audio interruption occurs.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class let interruptionNotification: NSNotification.Name
```

## Mentioned in 

Handling audio interruptions

## Discussion

The notification’s user-information dictionary contains the AVAudioSessionInterruptionTypeKey key. If the interruption type is AVAudioSession.InterruptionType.began, the system interrupted your app’s audio session and it’s no longer active. If the interruption type is AVAudioSession.InterruptionType.ended, this dictionary also contains the AVAudioSessionInterruptionOptionKey key.

See Handling audio interruptions for more information on using this notification.

The system posts this notification on the main thread.

Note

Starting in iOS 10, the system deactivates an app’s audio session when it suspends the app process. When the app starts running again, it receives an interruption notification that the system has deactivated its audio session. This notification is necessarily delayed in time because the system can only deliver it once the app is running again. If the system suspended your app’s audio session for this reason, the user-information dictionary contains the AVAudioSessionInterruptionWasSuspendedKey key with a value of true.

If you configured your audio session to be nonmixable (the default behavior for the playback, playAndRecord, soloAmbient, and multiRoute categories), deactivate your audio session if you’re not actively using audio when you go into the background. Doing so avoids having your audio session deactivated by the system (and receiving this somewhat confusing notification).

## Topics

### User Info Keys

let AVAudioSessionInterruptionTypeKey: String

A user info key to retrieve the interruption type.

let AVAudioSessionInterruptionOptionKey: String

A user info key to retrieve the interruption option.

let AVAudioSessionInterruptionReasonKey: String

A user info key to retrieve the interruption reason.

let AVAudioSessionInterruptionWasSuspendedKey: String

A user info key used to determine if the interruption is due to the audio session being deactivated when the system suspended the app.

Deprecated

### User Info Values

enum InterruptionType

Constants that describe the type of an audio interruption.

struct InterruptionOptions

Constants that indicate the state of an audio session after an interruption.

enum InterruptionReason

Constants that define the reasons for an audio session interruption.

## See Also

### Handling interruptions

var prefersNoInterruptionsFromSystemAlerts: Bool

A Boolean value that indicates a preference for not interrupting the session with system alerts.

func setPrefersNoInterruptionsFromSystemAlerts(Bool) throws

Sets the preference for not interrupting the audio session with system alerts.

var prefersInterruptionOnRouteDisconnect: Bool

A Boolean value that indicates whether the system interrupts the audio session when the active route disconnects.

func setPrefersInterruptionOnRouteDisconnect(Bool) throws

Sets a preference to interrupt the audio session when the active route disconnects.

