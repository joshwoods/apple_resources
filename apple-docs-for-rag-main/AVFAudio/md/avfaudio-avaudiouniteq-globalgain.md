

- AVFAudio
- AVAudioUnitEQ
-  globalGain 

Instance Property

# globalGain

The overall gain adjustment that the audio unit applies to the signal, in decibels.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var globalGain: Float { get set }
```

## Discussion

The default value is `0 db`. The valid range of values is `-96 db` to `24 db`.

## See Also

### Getting and setting the equalizer values

class AVAudioUnitEQFilterParameters

An object that encapsulates the parameters that the equalizer uses.

var bands: [AVAudioUnitEQFilterParameters]

An array of equalizer filter parameters.

