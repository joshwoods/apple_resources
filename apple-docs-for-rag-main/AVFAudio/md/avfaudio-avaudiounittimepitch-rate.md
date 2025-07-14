

- AVFAudio
- AVAudioUnitTimePitch
-  rate 

Instance Property

# rate

The playback rate of the input signal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var rate: Float { get set }
```

## Discussion

The default value is 1.0. The range of supported values is `1/32` to `32.0`.

## See Also

### Getting and setting time pitch values

var overlap: Float

The amount of overlap between segments of the input audio signal.

var pitch: Float

The amount to use to pitch shift the input signal.

