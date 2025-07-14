

- AVFAudio
- AVAudioUnitTimePitch
-  pitch 

Instance Property

# pitch

The amount to use to pitch shift the input signal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var pitch: Float { get set }
```

## Discussion

The audio unit measures the pitch in *cents*, a logarithmic value you use for measuring musical intervals. One octave is equal to 1200 cents. One musical semitone is equal to 100 cents.

The default value is ``` 0``.0 ```. The range of values is `-2400` to `2400`.

## See Also

### Getting and setting time pitch values

var overlap: Float

The amount of overlap between segments of the input audio signal.

var rate: Float

The playback rate of the input signal.

