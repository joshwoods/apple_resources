

- AVFAudio
- AVAudioUnitTimePitch
-  overlap 

Instance Property

# overlap

The amount of overlap between segments of the input audio signal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var overlap: Float { get set }
```

## Discussion

A higher value results in fewer artifacts in the output signal. The default value is `8.0`. The range of values is `3.0` to `32.0`.

## See Also

### Getting and setting time pitch values

var pitch: Float

The amount to use to pitch shift the input signal.

var rate: Float

The playback rate of the input signal.

