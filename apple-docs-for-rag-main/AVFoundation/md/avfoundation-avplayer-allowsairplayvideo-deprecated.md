

- AVFoundation
- AVPlayer
-  allowsAirPlayVideo Deprecated

Instance Property

# allowsAirPlayVideo

A Boolean value that indicates whether the player allows AirPlay video playback.

tvOS 9.0–9.0Deprecated

``` source
@MainActor
var allowsAirPlayVideo: Bool { get set }
```

Deprecated

Use allowsExternalPlayback instead.

## Discussion

The default value is true.

## See Also

### Configuring AirPlay Behavior

var isAirPlayVideoActive: Bool

A Boolean value that indicates whether the player is playing video through AirPlay.

Deprecated

var usesAirPlayVideoWhileAirPlayScreenIsActive: Bool

A Boolean value that indicates whether the player automatically switches to AirPlay Video while AirPlay Screen is active.

Deprecated

