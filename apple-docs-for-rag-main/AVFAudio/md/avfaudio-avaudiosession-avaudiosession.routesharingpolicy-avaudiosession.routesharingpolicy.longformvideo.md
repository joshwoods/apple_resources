

- AVFAudio
- AVAudioSession
- AVAudioSession.RouteSharingPolicy
-  AVAudioSession.RouteSharingPolicy.longFormVideo 

Case

# AVAudioSession.RouteSharingPolicy.longFormVideo

A policy that routes output to the shared long-form video output.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case longFormVideo
```

## Discussion

Apps that play long-form video content can use this policy to play to the same output as other long-form video apps, such as the built-in TV app. These apps should also set the `AVInitialRouteSharingPolicy` key in their `Info.plist` to `LongFormVideo`. Video content not using this route sharing policy remains local to the playback device even when the system is routing long-form video content to AirPlay.

## See Also

### Route-sharing policies

case `default`

A policy that follows standard rules for routing audio output.

case longFormAudio

A policy that routes output to the shared long-form audio output.

case independent

A policy in which the route picker UI directs videos to a wireless route.

static var longForm: AVAudioSession.RouteSharingPolicy

A policy that routes output to the shared long-form audio output.

Deprecated

