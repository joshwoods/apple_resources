

- AVFoundation
- AVAudioTimePitchAlgorithm
-  varispeed 

Type Property

# varispeed

A high-quality time pitch algorithm that doesn’t perform pitch correction.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
static let varispeed: AVAudioTimePitchAlgorithm
```

## Discussion

The pitch varies with the rate, and supports variable rates from `1/32` to `32`.

## See Also

### Constants

static let timeDomain: AVAudioTimePitchAlgorithm

A modest quality time pitch algorithm that’s suitable for voice.

static let spectral: AVAudioTimePitchAlgorithm

A highest-quality time pitch algorithm that’s suitable for music.

static let lowQualityZeroLatency: AVAudioTimePitchAlgorithm

A low-quality and very low computationally intensive pitch algorithm.

Deprecated

