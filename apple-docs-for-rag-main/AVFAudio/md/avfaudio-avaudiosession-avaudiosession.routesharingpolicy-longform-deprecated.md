

- AVFAudio
- AVAudioSession
- AVAudioSession.RouteSharingPolicy
-  longForm Deprecated

Type Property

# longForm

A policy that routes output to the shared long-form audio output.

iOS 11.0–13.0DeprecatediPadOS 11.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 11.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 4.0–6.0Deprecated

``` source
static var longForm: AVAudioSession.RouteSharingPolicy { get }
```

Deprecated

Use AVAudioSession.RouteSharingPolicy.longFormAudio instead.

## Discussion

An audio session whose primary use case is as a music or podcast player may use this value to play to the same output as the Music and Podcasts apps. All applications on the system that use this policy have their audio routed to the same location.

## See Also

### Route-sharing policies

case `default`

A policy that follows standard rules for routing audio output.

case longFormAudio

A policy that routes output to the shared long-form audio output.

case longFormVideo

A policy that routes output to the shared long-form video output.

case independent

A policy in which the route picker UI directs videos to a wireless route.

