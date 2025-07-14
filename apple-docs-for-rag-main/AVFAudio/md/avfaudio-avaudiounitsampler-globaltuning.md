

- AVFAudio
- AVAudioUnitSampler
-  globalTuning 

Instance Property

# globalTuning

An adjustment for the tuning of all the played notes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var globalTuning: Float { get set }
```

## Discussion

The tuning unit is cents, and defaults to `0.0`. The range of valid values is `-2400` to `2400` cents.

## See Also

### Getting and Setting Sampler Values

var overallGain: Float

An adjustment for the gain of all the played notes, in decibels.

var stereoPan: Float

An adjustment for the stereo panning of all the played notes.

var masterGain: Float

An adjustment for the gain of all the played notes, in decibels.

Deprecated

