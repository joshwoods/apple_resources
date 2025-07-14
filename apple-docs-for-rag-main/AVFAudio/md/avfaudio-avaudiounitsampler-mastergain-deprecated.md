

- AVFAudio
- AVAudioUnitSampler
-  masterGain Deprecated

Instance Property

# masterGain

An adjustment for the gain of all the played notes, in decibels.

iOS 8.0–15.0DeprecatediPadOS 8.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.10–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var masterGain: Float { get set }
```

Deprecated

Use overallGain instead.

## Discussion

The default value is `0.0` dB, and the range of valid values is `-90.0` dB to `12.0` dB.

## See Also

### Getting and Setting Sampler Values

var globalTuning: Float

An adjustment for the tuning of all the played notes.

var overallGain: Float

An adjustment for the gain of all the played notes, in decibels.

var stereoPan: Float

An adjustment for the stereo panning of all the played notes.

