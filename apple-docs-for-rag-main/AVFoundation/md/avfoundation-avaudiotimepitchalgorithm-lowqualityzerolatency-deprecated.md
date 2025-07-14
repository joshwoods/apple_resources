

- AVFoundation
- AVAudioTimePitchAlgorithm
-  lowQualityZeroLatency Deprecated

Type Property

# lowQualityZeroLatency

A low-quality and very low computationally intensive pitch algorithm.

iOS 7.0–15.0DeprecatediPadOS 7.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedtvOS 9.0–15.0DeprecatedwatchOS 1.0–8.0Deprecated

``` source
static let lowQualityZeroLatency: AVAudioTimePitchAlgorithm
```

Deprecated

Use timeDomain instead.

## Discussion

This algorithm is suitable for brief fast-forward and rewind effects, as well as low-quality voice. The rate snaps to `{0.5, 0.666667, 0.8, 1.0, 1.25, 1.5, 2.0}`.

## See Also

### Constants

static let timeDomain: AVAudioTimePitchAlgorithm

A modest quality time pitch algorithm that’s suitable for voice.

static let varispeed: AVAudioTimePitchAlgorithm

A high-quality time pitch algorithm that doesn’t perform pitch correction.

static let spectral: AVAudioTimePitchAlgorithm

A highest-quality time pitch algorithm that’s suitable for music.

