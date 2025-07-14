

- AVFoundation
-  AVAudioTimePitchAlgorithm 

Structure

# AVAudioTimePitchAlgorithm

An algorithm used to set the audio pitch as the rate changes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVAudioTimePitchAlgorithm
```

## Topics

### Type Properties

static let lowQualityZeroLatency: AVAudioTimePitchAlgorithm

A low-quality and very low computationally intensive pitch algorithm.

Deprecated

static let spectral: AVAudioTimePitchAlgorithm

A highest-quality time pitch algorithm that’s suitable for music.

static let timeDomain: AVAudioTimePitchAlgorithm

A modest quality time pitch algorithm that’s suitable for voice.

static let varispeed: AVAudioTimePitchAlgorithm

A high-quality time pitch algorithm that doesn’t perform pitch correction.

### Initializers

init(rawValue: String)

Creates a new time pitch algorithm with a string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Time Pitch Algorithm Setting

var audioTimePitchAlgorithm: AVAudioTimePitchAlgorithm?

The processing algorithm used to manage audio pitch for scaled audio edits.

