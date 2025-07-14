

- AVFoundation
- AVPlayerItem
-  audioMix 

Instance Property

# audioMix

The audio mix parameters to be applied during playback.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
@NSCopying @MainActor
var audioMix: AVAudioMix? { get set }
```

## Discussion

An audio mix can only be used with file-based media and is not supported for use with media served using HTTP Live Streaming.

## See Also

### Configuring Audio

var audioTimePitchAlgorithm: AVAudioTimePitchAlgorithm

The processing algorithm used to manage audio pitch for scaled audio edits.

var allowedAudioSpatializationFormats: AVAudioSpatializationFormats

The source audio channel layouts the player item supports for spatialization.

struct AVAudioSpatializationFormats

A structure that defines the spatialization formats that a player item supports.

var isAudioSpatializationAllowed: Bool

A Boolean value that indicates whether the player item allows spatialized audio playback.

Deprecated

