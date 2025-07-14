

- AVFAudio
- AVAudioSession
- AVAudioSession.RouteSharingPolicy
-  AVAudioSession.RouteSharingPolicy.independent 

Case

# AVAudioSession.RouteSharingPolicy.independent

A policy in which the route picker UI directs videos to a wireless route.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
case independent
```

## Discussion

In iOS, the system sets this policy in cases where the user directs video to a wireless route using the route picker UI. Apps shouldn’t try to set this value directly.

## See Also

### Route-sharing policies

case `default`

A policy that follows standard rules for routing audio output.

case longFormAudio

A policy that routes output to the shared long-form audio output.

case longFormVideo

A policy that routes output to the shared long-form video output.

static var longForm: AVAudioSession.RouteSharingPolicy

A policy that routes output to the shared long-form audio output.

Deprecated

