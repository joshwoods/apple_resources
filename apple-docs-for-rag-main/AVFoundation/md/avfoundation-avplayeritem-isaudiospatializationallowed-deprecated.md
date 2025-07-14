

- AVFoundation
- AVPlayerItem
-  isAudioSpatializationAllowed Deprecated

Instance Property

# isAudioSpatializationAllowed

A Boolean value that indicates whether the player item allows spatialized audio playback.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.15–15.0Deprecated

``` source
@MainActor
var isAudioSpatializationAllowed: Bool { get set }
```

Deprecated

Use allowedAudioSpatializationFormats instead.

## See Also

### Configuring Audio Behavior

var volume: Float

The audio playback volume for the player.

var isMuted: Bool

A Boolean value that indicates whether the audio output of the player is muted.

var allowedAudioSpatializationFormats: AVAudioSpatializationFormats

The source audio channel layouts the player item supports for spatialization.

