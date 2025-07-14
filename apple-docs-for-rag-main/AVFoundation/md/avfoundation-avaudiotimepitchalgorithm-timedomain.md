

- AVFoundation
- AVAudioTimePitchAlgorithm
-  timeDomain 

Type Property

# timeDomain

A modest quality time pitch algorithm that’s suitable for voice.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
static let timeDomain: AVAudioTimePitchAlgorithm
```

## Discussion

This is less computationally intensive than spectral, and uses a variable rate from `1/32` to `32`.

## See Also

### Constants

static let varispeed: AVAudioTimePitchAlgorithm

A high-quality time pitch algorithm that doesn’t perform pitch correction.

static let spectral: AVAudioTimePitchAlgorithm

A highest-quality time pitch algorithm that’s suitable for music.

static let lowQualityZeroLatency: AVAudioTimePitchAlgorithm

A low-quality and very low computationally intensive pitch algorithm.

Deprecated

