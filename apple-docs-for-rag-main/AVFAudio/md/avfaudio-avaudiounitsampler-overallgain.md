

- AVFAudio
- AVAudioUnitSampler
-  overallGain 

Instance Property

# overallGain

An adjustment for the gain of all the played notes, in decibels.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var overallGain: Float { get set }
```

## Discussion

The default value is `0.0` dB, and the range of valid values is `-90.0` dB to `12.0` dB.

## See Also

### Getting and Setting Sampler Values

var globalTuning: Float

An adjustment for the tuning of all the played notes.

var stereoPan: Float

An adjustment for the stereo panning of all the played notes.

var masterGain: Float

An adjustment for the gain of all the played notes, in decibels.

Deprecated

