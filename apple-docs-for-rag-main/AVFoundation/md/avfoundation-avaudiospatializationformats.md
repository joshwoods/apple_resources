

- AVFoundation
-  AVAudioSpatializationFormats 

Structure

# AVAudioSpatializationFormats

A structure that defines the spatialization formats that a player item supports.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVAudioSpatializationFormats
```

## Topics

### Spatialization Formats

static var monoAndStereo: AVAudioSpatializationFormats

A value that indicates the player item only supports mono and stereo layouts for audio spatialization.

static var multichannel: AVAudioSpatializationFormats

A value that indicates the player item only supports multichannel layouts for audio spatialization.

static var monoStereoAndMultichannel: AVAudioSpatializationFormats

A value that indicates the player item supports mono, stereo, and multichannel layouts for audio spatialization.

### Initializers

init(rawValue: UInt)

Initializes a format with a string value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Configuring Audio

var audioMix: AVAudioMix?

The audio mix parameters to be applied during playback.

var audioTimePitchAlgorithm: AVAudioTimePitchAlgorithm

The processing algorithm used to manage audio pitch for scaled audio edits.

var allowedAudioSpatializationFormats: AVAudioSpatializationFormats

The source audio channel layouts the player item supports for spatialization.

var isAudioSpatializationAllowed: Bool

A Boolean value that indicates whether the player item allows spatialized audio playback.

Deprecated

