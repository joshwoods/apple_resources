

- AVFAudio
- AVAudioUnitDelay
-  wetDryMix 

Instance Property

# wetDryMix

The blend of the wet and dry signals.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var wetDryMix: Float { get set }
```

## Discussion

You specify the blend as a percentage. The default value is `100%`. The valid range of values is `0%` through `100%`, where `0%` represents all dry.

## See Also

### Getting and setting the delay values

var delayTime: TimeInterval

The time for the input signal to reach the output.

var feedback: Float

The amount of the output signal that feeds back into the delay line.

var lowPassCutoff: Float

The cutoff frequency above which high frequency content rolls off, in hertz.

