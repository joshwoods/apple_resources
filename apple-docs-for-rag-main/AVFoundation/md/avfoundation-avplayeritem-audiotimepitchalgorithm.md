

- AVFoundation
- AVPlayerItem
-  audioTimePitchAlgorithm 

Instance Property

# audioTimePitchAlgorithm

The processing algorithm used to manage audio pitch for scaled audio edits.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
var audioTimePitchAlgorithm: AVAudioTimePitchAlgorithm { get set }
```

## Discussion

The supported constants are defined in Time Pitch Algorithm Settings.

An invalidArgumentException will be raised if this property is set to a value other than the defined constants.

## See Also

### Configuring Audio

var audioMix: AVAudioMix?

The audio mix parameters to be applied during playback.

var allowedAudioSpatializationFormats: AVAudioSpatializationFormats

The source audio channel layouts the player item supports for spatialization.

struct AVAudioSpatializationFormats

A structure that defines the spatialization formats that a player item supports.

var isAudioSpatializationAllowed: Bool

A Boolean value that indicates whether the player item allows spatialized audio playback.

Deprecated

