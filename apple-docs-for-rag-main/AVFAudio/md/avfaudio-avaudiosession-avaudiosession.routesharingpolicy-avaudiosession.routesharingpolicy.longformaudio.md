

- AVFAudio
- AVAudioSession
- AVAudioSession.RouteSharingPolicy
-  AVAudioSession.RouteSharingPolicy.longFormAudio 

Case

# AVAudioSession.RouteSharingPolicy.longFormAudio

A policy that routes output to the shared long-form audio output.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
case longFormAudio
```

## Discussion

Apps that play long-form audio, such as music or audio books, can use this policy to play to the same output as the built-in Music and Podcast apps. Long-form audio apps should also use the Media Player framework to add support for remote control events and to provide Now Playing information.

Apps running in watchOS that use this policy are able to play audio in the background, as long as the audio session can activate an eligible audio route. These apps must activate their audio session using the activate(options:completionHandler:) method. This ensures that the user has the opportunity to pick an appropriate audio route when the audio session can’t select one automatically.

## See Also

### Route-sharing policies

case `default`

A policy that follows standard rules for routing audio output.

case longFormVideo

A policy that routes output to the shared long-form video output.

case independent

A policy in which the route picker UI directs videos to a wireless route.

static var longForm: AVAudioSession.RouteSharingPolicy

A policy that routes output to the shared long-form audio output.

Deprecated

