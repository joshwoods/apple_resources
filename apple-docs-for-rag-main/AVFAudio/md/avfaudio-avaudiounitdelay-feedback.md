

- AVFAudio
- AVAudioUnitDelay
-  feedback 

Instance Property

# feedback

The amount of the output signal that feeds back into the delay line.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var feedback: Float { get set }
```

## Discussion

You specify the feedback as a percentage. The default value is `50%`. The valid range of values is `-100%` to `100%`.

## See Also

### Getting and setting the delay values

var delayTime: TimeInterval

The time for the input signal to reach the output.

var lowPassCutoff: Float

The cutoff frequency above which high frequency content rolls off, in hertz.

var wetDryMix: Float

The blend of the wet and dry signals.

