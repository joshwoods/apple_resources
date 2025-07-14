

- AVFAudio
- AVAudioUnitDelay
-  delayTime 

Instance Property

# delayTime

The time for the input signal to reach the output.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var delayTime: TimeInterval { get set }
```

## Discussion

You specify the delay in seconds. The default value is `1`. The valid range of values is `0` to `2` seconds.

## See Also

### Getting and setting the delay values

var feedback: Float

The amount of the output signal that feeds back into the delay line.

var lowPassCutoff: Float

The cutoff frequency above which high frequency content rolls off, in hertz.

var wetDryMix: Float

The blend of the wet and dry signals.

