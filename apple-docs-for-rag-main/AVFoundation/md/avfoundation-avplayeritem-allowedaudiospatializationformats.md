

- AVFoundation
- AVPlayerItem
-  allowedAudioSpatializationFormats 

Instance Property

# allowedAudioSpatializationFormats

The source audio channel layouts the player item supports for spatialization.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 15.0+visionOS 1.0+

``` source
nonisolated
var allowedAudioSpatializationFormats: AVAudioSpatializationFormats { get set }
```

## Discussion

Spatialization uses psychoacoustic methods to create a more immersive audio experience when playing content on specialized headphones and speaker arrangements.

The default value for video content is monoStereoAndMultichannel, and multichannel for audio-only content. Your app can set a preferred spatialization format, but a user can change the audio spatialization behavior in Control Center.

This property isn’t key-value observable.

Important

It’s incorrect to render binaural recordings with spatialization. Content tagged with a binaural channel layout ignores this property value.

## See Also

### Configuring Audio Behavior

var volume: Float

The audio playback volume for the player.

var isMuted: Bool

A Boolean value that indicates whether the audio output of the player is muted.

var isAudioSpatializationAllowed: Bool

A Boolean value that indicates whether the player item allows spatialized audio playback.

Deprecated

